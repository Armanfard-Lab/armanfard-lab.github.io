---
title: "ASTAD - AAAI-27"
layout: gridlay2
excerpt: "ASTAD - AAAI-27"
sitemap: false
permalink: /astad4/
---

<div style="margin: 0 auto 20px; text-align: center;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad4_banner.jpg" alt="Palais des Congrès de Montréal, AAAI-27 venue" style="width: 100%; max-width: 1100px; height: auto; display: block; margin: 0 auto; border-radius: 12px;" />
</div>

<h1 align="center"> 4th Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) </h1>

<div style="padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad_aaai27_logo.png" alt="iSMART Lab and AAAI-27, Montréal" style="width: 500px; max-width: 95vw; height: auto; display: block; margin: 0 auto;" />
</div>

<h2 align="center">Overview</h2>
<hr>

<p align="center">The 4th Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) at AAAI-27 brings together researchers and practitioners working on AI-driven anomaly detection across images and video, signals and time series, and graphs. As detection moves from curated benchmarks into deployed systems, anomalies often appear only in the relationship between data streams, such as images, sensor readings, event logs, and maintenance records. ASTAD welcomes work that bridges modalities, disciplines, and method families. This year, the scope extends to detection-specific foundation models, generalist detectors, reasoning-based detection, agentic pipelines that carry detection through to root-cause analysis, and anomaly detection in deployed autonomous agents.</p>

<h2 align="center"> Call for Papers </h2>
<hr>

<p align="left">We invite researchers and practitioners to submit their original research contributions to the 4th Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of AAAI-27. Topics include, but are not limited to:</p>

  <ul>
    <li> Novel architectures and deep generative models for anomaly detection in images, video, graphs, signals, and tabular data, including anomaly synthesis </li>
    <li> Foundation models, vision–language models, and multimodal LLMs for anomaly detection, including generalist detectors </li>
    <li> Agentic anomaly detection and root-cause analysis; anomaly detection in deployed autonomous agents </li>
    <li> Self-supervised, unsupervised, few-shot, zero-shot, and continual anomaly detection under distribution shift </li>
    <li> Explainable and reasoning-based anomaly detection </li>
    <li> Datasets and benchmarking, including zero-shot data leakage and negative results </li>
    <li> Real-time and on-edge anomaly detection </li>
    <li> Applications in healthcare, industry, automotive, robotics, remote sensing, energy, and finance </li>
  </ul>

<h3 align="left"> Submission Requirements </h3>

<p align="left">We welcome original research as full papers of up to 8 pages or short and position papers of up to 4 pages, plus additional pages for references only. Submissions must use the official AAAI-27 author kit and will undergo double-blind peer review. We plan to publish accepted papers in proceedings; details will be posted on this page.</p>

<p align="left">All submissions will be handled electronically via OpenReview. Only PDF files are accepted.</p>

<p align="left">Submission Site: <a href="https://openreview.net/group?id=AAAI.org/2027/Workshop/ASTAD" target="_blank">OpenReview</a></p>

<h2 align="center"> Format </h2>
<hr>

<p align="left">ASTAD is a one-day event combining paper presentations, invited talks from leading researchers, and interactive poster sessions, with ample time for Q&amp;A and discussion.</p>

<h2 align="center"> Important Dates </h2>
<hr>

<ul>
 <li> <b>Paper submission deadline:</b> November 20, 2026 </li>
 <li> <b>Author notification:</b> December 2, 2026 </li>
 <li> <b>Camera-ready deadline:</b> To be announced </li>
 <li> <b>Workshop Date:</b> February 22–23, 2027 </li>
 <li> <b>Workshop Location:</b> Montréal, Canada </li>
</ul>

<h2 align="center"> Schedule </h2>
<hr>

<p align="center">The workshop schedule will be announced soon.</p>

<h2 align="center"> Speakers </h2>
<hr>

<p align="center">Keynote speakers will be announced soon.</p>

<h2 align="center">Workshop Poster</h2>
<hr>

<div style="padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad4_poster.png" style="width: 800px; max-width: 95vw; height: auto; display: block; margin: 0 auto; border-radius: 0;" />
</div>

<h2 align="center"> Organizers </h2>
<hr>

{% assign number_printed = 0 %}
{% for member in site.data.ijcaimember %}
{% if member.name == "Narges Armanfard (Chair)" %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} - {{ member.email }}</i>
  <p style="font-size:14px;">{{ member.bio }}</p>
  <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>
{% endif %}
{% endfor %}

{% for member in site.data.team_members %}
{% if member.name == "Thi Kieu Khanh Ho" or member.name == "Thomas Lai" %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} - {{ member.email }}</i>
  <p style="font-size:14px;">{{ member.bio }}</p>
  <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>
{% endif %}
{% endfor %}
