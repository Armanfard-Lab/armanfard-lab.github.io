---
title: "ASTAD - AAAI-26"
layout: gridlay2
excerpt: "ASTAD - AAAI-26"
sitemap: false
permalink: /astad3/
---

<h1 align="center"> 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) </h1>



{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
  
  <div style="border-radius: 16px; padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad_aaai26_logo.png" style="width: 500px; max-width: 95vw; height: auto; display: block; margin: 0 auto;" />
</div>


 

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}

<h2 align="center">Overview</h2>
<hr>

<p align="center">The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) at AAAI 2026 is a premier platform for researchers and practitioners at the forefront of AI-driven anomaly detection. With the proliferation of spatiotemporal data from sources like surveillance cameras, IoT sensors, and satellite imagery, the need for robust, automated systems to identify novel and unusual patterns has never been more critical. This workshop will delve into cutting-edge AI techniques that move beyond traditional rule-based methods to uncover hidden anomalies, fostering a new generation of intelligent monitoring and discovery. Join us to discuss how we can build more resilient, autonomous, and insightful systems for a safer and more efficient world.</p>

<h2 align="center"> Call for Paper </h2>
<hr>
  
<p align="left">We invite researchers and practitioners to submit their original research contributions to The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of AAAI 2026. This workshop aims to explore the latest advancements and novel approaches in anomaly detection (AD) using Artificial Intelligence techniques, with a focus on spatial and temporal dimensions. Topics of Interest :</p>
  
  <ul>
    <li> Novel deep learning and generative models for spatiotemporal AD </li>
    <li> Self-supervised, unsupervised and few-shot learning for AD with limited data </li>
    <li> Continual learning approaches for evolving anomalous patterns </li>
    <li> Explainable AI for interpreting and justifying anomaly detection decisions </li>
    <li> Foundation models for anomaly detection, including large language models (LLMs) and vision-language models (VLMs) </li>
    <li> Novel datasets, benchmarks, and evaluation metrics </li>
    <li> On-edge anomaly detection in real-time and resource-constrained settings </li>
    <li> Applications in computer vision, robotics, autonomous driving, predictive maintenance, healthcare, finance, and beyond </li>
  </ul>  

<p align="left">Submission Site: <a href="https://openreview.net/group?id=AAAI.org/2026/Workshop/ASTAD" target="_blank">OpenReview</a></p>


<h2 align="center"> Schedule </h2>
<hr>

Coming Soon

<h2 align="center"> Important Dates </h2>
<hr>

   <p align="left"> The important dates are as follows: </p>
<ul>
<li> <b>Paper submission deadline:</b> October 22, 2025 </li>
 <li> <b>Author notification:</b> November 5, 2025 </li>
 <li> <b>Camera-ready deadline:</b> November 10, 2025 </li>
  </ul>

  <h2 align="center"> Speakers </h2>
<hr>

Coming Soon

<h2 align="center">Workshop Poster</h2>
<hr>

<div style="padding: 20px 24px; margin: 20px auto; text-align: center; display: block; width: fit-content;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad3_poster.png" style="width: 800px; max-width: 95vw; height: auto; display: block; margin: 0 auto; border-radius: 0;" />
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
{% if member.name == "Hadi Hojjati" or member.name == "Thi Kieu Khanh Ho" %}

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

 