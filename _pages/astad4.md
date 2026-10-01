---
title: "ASTAD - AAAI-27"
layout: gridlay2
excerpt: "ASTAD - AAAI-27"
sitemap: false
permalink: /astad4/
---

<div style="padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad4_title_banner.png" alt="4th Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), iSMART Lab, AAAI-27, Feb 16-23 2027, Montréal, Canada" style="width: 900px; max-width: 95vw; height: auto; display: block; margin: 0 auto;" />
</div>

<h2 align="center">Overview</h2>
<hr>

<p align="center">ASTAD brings together researchers and practitioners working on AI methods for detecting, predicting, explaining, and responding to anomalies, abnormalities, outliers, risks, failures, and deviations from expected or learned normal behavior across spatial, temporal, and multimodal data. The workshop welcomes methodological advances as well as real-world applications in industry, IT systems, finance, healthcare, and beyond, spanning anomaly detection and prediction, out-of-distribution and outlier detection, fraud detection, predictive maintenance, risk analysis and assessment, fault and failure detection/prediction, accident and incident detection/prediction, early warning systems, and abnormal behavior recognition.</p>

<h2 align="center"> Call for Papers </h2>
<hr>

<p align="left">We invite researchers and practitioners to submit their original research contributions to the 4th Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of AAAI-27. Topics include, but are not limited to:</p>

  <ul>
    <li> Anomaly, abnormality, novelty, outlier, and out-of-distribution detection </li>
    <li> Anomaly and abnormal-event prediction / forecasting </li>
    <li> Predictive maintenance, fault diagnosis, and failure prediction in industrial and IT systems </li>
    <li> Risk analysis, risk prediction, and early-warning systems in healthcare, finance, and infrastructure </li>
    <li> Fraud detection and financial anomaly detection </li>
    <li> Accident, incident, and hazard detection and prediction </li>
    <li> Detection and prediction of deviations from expected or learned normal behavior </li>
    <li> Root-cause analysis, diagnosis, localization, and attribution across clinical, industrial, and IT settings </li>
    <li> Foundation models, LLMs, VLMs, and generalist models for detection and prediction </li>
    <li> Agentic AI for monitoring, diagnosis, prediction, and autonomous response </li>
    <li> Generative, self-supervised, unsupervised, few-shot, and zero-shot approaches </li>
    <li> Explainable, interpretable, causal, and reasoning-based methods </li>
    <li> Multimodal, spatial, temporal, spatiotemporal, graph, image, video, signal, and tabular data </li>
    <li> Real-time, streaming, continual, and on-device methods </li>
    <li> Datasets, benchmarks, evaluation, uncertainty, robustness, and distribution shift </li>
    <li> Applications in healthcare, manufacturing, IT operations, automotive, transportation, robotics, cybersecurity, remote sensing, infrastructure, energy, finance, and safety-critical systems </li>
  </ul>

<h3 align="left"> Submission Requirements </h3>

<p align="left">We welcome original research as full papers of up to 7 pages, plus 2 additional pages for references only. Submissions must use the official AAAI-27 author kit and will undergo double-blind peer review.</p>

<p align="left">All submissions will be handled electronically via OpenReview. Only PDF files are accepted.</p>

<p align="left">Submission Site: <a href="https://openreview.net/group?id=AAAI.org/2027/Workshop/ASTAD" target="_blank">OpenReview</a></p>

<h2 align="center"> Format </h2>
<hr>

<p align="left">ASTAD is a one-day event combining paper presentations, invited talks from leading researchers, and interactive poster sessions, with ample time for Q&amp;A and discussion.</p>

<h2 align="center"> Attendance </h2>
<hr>

<p align="left">Attendance is open to all registered AAAI-27 participants, including researchers, students, and industry professionals.</p>

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
