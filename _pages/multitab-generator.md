---
title: "MultiTab — Synthetic Dataset Generator"
layout: default
excerpt: "MultiTab Synthetic Dataset Generator"
sitemap: true
permalink: /multitab-generator/
---

<div class="col-sm-12" style="max-width: 900px; margin: 0 auto; padding: 30px 15px;">

<h2 style="text-align:center; margin-bottom: 6px;">MultiTab — Synthetic Dataset Generator</h2>
<p style="text-align:center; color: #666; margin-bottom: 30px;">Generate multitask tabular data with controllable task correlations, polynomial complexity, and noise.</p>

<form id="multitab-form" onsubmit="return false;">

  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px 24px; margin-bottom: 20px;">

    <div>
      <label for="mt-name"><strong>Dataset name</strong></label>
      <input id="mt-name" type="text" class="form-control" value="synthetic_v2">
    </div>

    <div>
      <label for="mt-short-name"><strong>Short name</strong></label>
      <input id="mt-short-name" type="text" class="form-control" value="syn_v2">
    </div>

    <div>
      <label for="mt-num-tasks"><strong>Number of tasks (T)</strong></label>
      <input id="mt-num-tasks" type="number" class="form-control" value="7" min="1" max="50">
    </div>

    <div>
      <label for="mt-num-features"><strong>Number of features (D)</strong></label>
      <input id="mt-num-features" type="number" class="form-control" value="32" min="1" max="500">
    </div>

    <div>
      <label for="mt-correlation"><strong>Correlation (ρ)</strong></label>
      <input id="mt-correlation" type="number" class="form-control" value="0.4" step="0.01" min="-1" max="1">
    </div>

    <div>
      <label for="mt-num-samples"><strong>Number of samples</strong></label>
      <input id="mt-num-samples" type="number" class="form-control" value="10000" min="100" max="200000">
      <small class="text-muted">Max 200,000 in-browser.</small>
    </div>

    <div>
      <label for="mt-split"><strong>Train/test split</strong></label>
      <input id="mt-split" type="number" class="form-control" value="0.7" step="0.05" min="0.1" max="0.95">
    </div>

  </div>

  <div style="margin-bottom: 16px;">
    <label for="mt-poly-degrees"><strong>Polynomial degrees</strong> <small class="text-muted">(comma-separated, one per task)</small></label>
    <input id="mt-poly-degrees" type="text" class="form-control" value="1, 3, 2, 3, 4, 2, 3">
  </div>

  <div style="margin-bottom: 24px;">
    <label for="mt-noise-levels"><strong>Noise levels (σ)</strong> <small class="text-muted">(comma-separated, one per task)</small></label>
    <input id="mt-noise-levels" type="text" class="form-control" value="0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01">
  </div>

  <div style="text-align: center; margin-bottom: 12px;">
    <button id="mt-generate-btn" type="button" class="btn btn-danger" style="background-color: #9E0918; border-color: #9E0918; padding: 10px 40px; font-size: 16px;" onclick="generateDataset()">
      Generate &amp; Download CSV
    </button>
  </div>

  <div id="mt-status" style="text-align:center; margin-top: 10px; color: #555;"></div>
  <div id="mt-error" style="text-align:center; margin-top: 10px; color: #c00;"></div>

</form>

<hr style="margin: 30px 0;">

<details style="margin-bottom: 20px;">
<summary style="cursor:pointer; font-weight:bold;">How it works</summary>
<div style="padding: 12px 0; font-size: 14px; line-height: 1.7;">
<p>The generator creates a multitask regression dataset where task weight vectors share a controlled pairwise cosine similarity <strong>ρ</strong>.</p>
<ol>
<li>Orthogonal unit vectors <strong>U</strong> are constructed via Gram–Schmidt.</li>
<li>A Gram matrix <strong>P</strong> is built with off-diagonal entries = ρ.</li>
<li>Eigendecomposition of <strong>P</strong> yields the weight matrix <strong>W = V √Λ U</strong>.</li>
<li>Input features <strong>X</strong> are sampled from N(0, 1).</li>
<li>Labels for task <em>t</em>: y<sub>t</sub> = Xw<sub>t</sub> + Σ<sub>k=2…d</sub> (Xw<sub>t</sub>)<sup>k</sup> + ε, where ε ~ N(0, σ²).</li>
</ol>
<p>The output CSV contains columns <code>x_0, x_1, …, x_{D-1}, task_0, task_1, …, task_{T-1}, split</code> where <code>split</code> is <code>train</code> or <code>test</code>.</p>
</div>
</details>

<p style="text-align: center; color: #888; font-size: 13px;">
  Need more than 200K samples? Use the
  <a href="https://colab.research.google.com/" target="_blank" style="color: #9E0918;">Google Colab notebook</a> (coming soon).
</p>

</div>

<script>
(function () {
  "use strict";

  function randn() {
    var u = 0, v = 0;
    while (u === 0) u = Math.random();
    while (v === 0) v = Math.random();
    return Math.sqrt(-2.0 * Math.log(u)) * Math.cos(2.0 * Math.PI * v);
  }

  function randnMatrix(rows, cols) {
    var m = new Float64Array(rows * cols);
    for (var i = 0; i < m.length; i++) m[i] = randn();
    return { data: m, rows: rows, cols: cols };
  }

  function dot(a, aOff, b, bOff, len) {
    var s = 0;
    for (var i = 0; i < len; i++) s += a[aOff + i] * b[bOff + i];
    return s;
  }

  function gramSchmidt(T, D) {
    var U = randnMatrix(T, D);
    for (var i = 0; i < T; i++) {
      var ri = i * D;
      for (var j = 0; j < i; j++) {
        var rj = j * D;
        var d = dot(U.data, ri, U.data, rj, D);
        for (var k = 0; k < D; k++) U.data[ri + k] -= d * U.data[rj + k];
      }
      var norm = Math.sqrt(dot(U.data, ri, U.data, ri, D));
      for (var k = 0; k < D; k++) U.data[ri + k] /= norm;
    }
    return U;
  }

  function jacobiEigen(A, n) {
    var V = new Float64Array(n * n);
    var S = new Float64Array(n * n);
    for (var i = 0; i < n * n; i++) S[i] = A[i];
    for (var i = 0; i < n; i++) V[i * n + i] = 1;

    for (var iter = 0; iter < 100; iter++) {
      var offDiag = 0;
      for (var p = 0; p < n; p++)
        for (var q = p + 1; q < n; q++)
          offDiag += S[p * n + q] * S[p * n + q];
      if (offDiag < 1e-15) break;

      for (var p = 0; p < n; p++) {
        for (var q = p + 1; q < n; q++) {
          if (Math.abs(S[p * n + q]) < 1e-15) continue;
          var tau = (S[q * n + q] - S[p * n + p]) / (2 * S[p * n + q]);
          var t = ((tau >= 0) ? 1 : -1) / (Math.abs(tau) + Math.sqrt(1 + tau * tau));
          var c = 1 / Math.sqrt(1 + t * t);
          var s = t * c;

          var app = S[p * n + p], aqq = S[q * n + q], apq = S[p * n + q];
          S[p * n + p] = app - t * apq;
          S[q * n + q] = aqq + t * apq;
          S[p * n + q] = 0;
          S[q * n + p] = 0;

          for (var r = 0; r < n; r++) {
            if (r === p || r === q) continue;
            var rp = S[r * n + p], rq = S[r * n + q];
            S[r * n + p] = c * rp - s * rq;
            S[p * n + r] = S[r * n + p];
            S[r * n + q] = s * rp + c * rq;
            S[q * n + r] = S[r * n + q];
          }
          for (var r = 0; r < n; r++) {
            var vp = V[r * n + p], vq = V[r * n + q];
            V[r * n + p] = c * vp - s * vq;
            V[r * n + q] = s * vp + c * vq;
          }
        }
      }
    }

    var eigvals = new Float64Array(n);
    for (var i = 0; i < n; i++) eigvals[i] = S[i * n + i];
    return { values: eigvals, vectors: V, n: n };
  }

  function buildWeightMatrix(T, D, correlation) {
    var U = gramSchmidt(T, D);

    var P = new Float64Array(T * T);
    for (var i = 0; i < T; i++)
      for (var j = 0; j < T; j++)
        P[i * T + j] = (i === j) ? 1.0 : correlation;

    var eig = jacobiEigen(P, T);

    // W = V * diag(sqrt(lambda)) * U   →  W is T×D
    var W = new Float64Array(T * D);
    for (var i = 0; i < T; i++) {
      var sqrtLam = new Float64Array(T);
      for (var k = 0; k < T; k++)
        sqrtLam[k] = eig.vectors[i * T + k] * Math.sqrt(Math.max(eig.values[k], 0));
      for (var d = 0; d < D; d++) {
        var s = 0;
        for (var k = 0; k < T; k++) s += sqrtLam[k] * U.data[k * D + d];
        W[i * D + d] = s;
      }
    }
    return W;
  }

  function generateLabels(X, W, N, D, T, polyDegrees, noiseLevels) {
    var Y = new Float64Array(N * T);
    for (var t = 0; t < T; t++) {
      var wOff = t * D;
      var deg = polyDegrees[t];
      var sigma = noiseLevels[t];
      for (var i = 0; i < N; i++) {
        var lin = 0;
        for (var d = 0; d < D; d++) lin += X[i * D + d] * W[wOff + d];
        var val = lin;
        if (deg >= 2) {
          var pw = lin;
          for (var k = 2; k <= deg; k++) {
            pw *= lin;
            val += pw;
          }
        }
        val += randn() * sigma;
        Y[i * T + t] = val;
      }
    }
    return Y;
  }

  function buildCSV(X, Y, N, D, T, split) {
    var trainN = Math.floor(N * split);
    var parts = [];
    var header = [];
    for (var d = 0; d < D; d++) header.push("x_" + d);
    for (var t = 0; t < T; t++) header.push("task_" + t);
    header.push("split");
    parts.push(header.join(","));

    for (var i = 0; i < N; i++) {
      var row = [];
      for (var d = 0; d < D; d++) row.push(X[i * D + d].toFixed(6));
      for (var t = 0; t < T; t++) row.push(Y[i * T + t].toFixed(6));
      row.push(i < trainN ? "train" : "test");
      parts.push(row.join(","));
    }
    return parts.join("\n");
  }

  function parseList(str, n, fallback) {
    var parts = str.split(",").map(function (s) { return parseFloat(s.trim()); });
    if (parts.length === 1 && !isNaN(parts[0])) {
      var arr = [];
      for (var i = 0; i < n; i++) arr.push(parts[0]);
      return arr;
    }
    if (parts.length !== n || parts.some(isNaN)) return null;
    return parts;
  }

  window.generateDataset = function () {
    var errEl = document.getElementById("mt-error");
    var statEl = document.getElementById("mt-status");
    errEl.textContent = "";
    statEl.textContent = "";

    var T = parseInt(document.getElementById("mt-num-tasks").value);
    var D = parseInt(document.getElementById("mt-num-features").value);
    var rho = parseFloat(document.getElementById("mt-correlation").value);
    var N = parseInt(document.getElementById("mt-num-samples").value);
    var split = parseFloat(document.getElementById("mt-split").value);
    var name = document.getElementById("mt-name").value.trim() || "synthetic";

    if (isNaN(T) || T < 1) { errEl.textContent = "Number of tasks must be ≥ 1."; return; }
    if (isNaN(D) || D < T) { errEl.textContent = "Number of features must be ≥ number of tasks (for orthogonal vectors)."; return; }
    if (isNaN(rho) || rho < -1 || rho > 1) { errEl.textContent = "Correlation must be between -1 and 1."; return; }
    if (isNaN(N) || N < 100 || N > 200000) { errEl.textContent = "Number of samples must be between 100 and 200,000."; return; }
    if (isNaN(split) || split < 0.1 || split > 0.95) { errEl.textContent = "Split must be between 0.1 and 0.95."; return; }

    var polyDegrees = parseList(document.getElementById("mt-poly-degrees").value, T);
    if (!polyDegrees) { errEl.textContent = "Polynomial degrees: enter " + T + " comma-separated integers (or one value for all)."; return; }

    var noiseLevels = parseList(document.getElementById("mt-noise-levels").value, T);
    if (!noiseLevels) { errEl.textContent = "Noise levels: enter " + T + " comma-separated numbers (or one value for all)."; return; }

    statEl.textContent = "Generating " + N.toLocaleString() + " samples …";
    var btn = document.getElementById("mt-generate-btn");
    btn.disabled = true;

    setTimeout(function () {
      try {
        var t0 = performance.now();
        var W = buildWeightMatrix(T, D, rho);
        var Xm = randnMatrix(N, D);
        var Y = generateLabels(Xm.data, W, N, D, T, polyDegrees, noiseLevels);
        var csv = buildCSV(Xm.data, Y, N, D, T, split);
        var elapsed = ((performance.now() - t0) / 1000).toFixed(1);

        var blob = new Blob([csv], { type: "text/csv" });
        var url = URL.createObjectURL(blob);
        var a = document.createElement("a");
        a.href = url;
        a.download = name + ".csv";
        document.body.appendChild(a);
        a.click();
        document.body.removeChild(a);
        URL.revokeObjectURL(url);

        statEl.textContent = "Done in " + elapsed + "s — " + N.toLocaleString() + " × " + (D + T) + " values downloaded.";
      } catch (e) {
        errEl.textContent = "Error: " + e.message;
      }
      btn.disabled = false;
    }, 50);
  };
})();
</script>
