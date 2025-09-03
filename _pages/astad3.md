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
  <img src="{{ site.url }}{{ site.baseurl }}/images/astad_aaai26_logo.png" style="width: 320px; max-width: 95vw; height: auto; display: block; margin: 0 auto;" />
</div>

  <h2 align="center">Description of Workshop</h2>
   <hr>
  <p align="center">The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) at AAAI-26 is a premier platform for researchers and practitioners at the forefront of AI-driven anomaly detection. With the proliferation of spatiotemporal data from sources like surveillance cameras, IoT sensors, and satellite imagery, the need for robust, automated systems to identify novel and unusual patterns has never been more critical. This workshop will delve into cutting-edge AI techniques that move beyond traditional rule-based methods to uncover hidden anomalies, fostering a new generation of intelligent monitoring and discovery. Join us to discuss how we can build more resilient, autonomous, and insightful systems for a safer and more efficient world.</p>
 

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endfor %}

<h2 align="center">Topics</h2>
<hr>
  
<p align="left">We invite submissions on a wide range of topics, including but not limited to:</p>
  
  <ul>
    <li> Novel deep learning and generative models for spatiotemporal anomaly detection. </li>
    <li> Self-supervised, unsupervised, and few-shot learning for anomaly detection with limited data. </li>
    <li> Continual and lifelong learning approaches to adapt to evolving anomalous patterns. </li>
    <li> Explainable AI (XAI) for interpreting and justifying anomaly detection decisions. </li>
    <li> The role of Large-Language Models (LLMs) and foundation models in anomaly detection. </li>
    <li> Novel datasets, benchmarks, and evaluation metrics. </li>
    <li> Applications in computer vision, robotics, healthcare, finance, and beyond. </li>
  </ul>  

<h2 align="center">Format of Workshop</h2>
<hr>

<p align="left">ASTAD will be a dynamic one-day event designed for maximum engagement and knowledge exchange. The format will include a mix of paper presentations, invited talks from leading researchers, and interactive poster sessions. We aim to spark lively discussion and debate by dedicating ample time to Q&A and a concluding panel discussion with organizers and invited speakers. This structure is designed to not only showcase new research but also to build a vibrant community around this critical topic.</p>

<h2 align="center">Attendance</h2>
<hr>

<p align="left">Attendance is open to all registered participants of the AAAI-26 conference. We encourage anyone with an interest in the topic to attend, whether you are a researcher, a student, or an industry professional.</p>

<h2 align="center">Submission Requirements</h2>
<hr>

<p align="left">We welcome original research contributions as full papers, in line with the standards of AAAI main track format. Submissions may consist of up to 7 pages of technical content plus additional pages solely for references. All submissions must be formatted using the official AAAI-26 author kit and will be subject to a double-blind peer-review process. Accepted papers will be included in the non-archival workshop proceedings, allowing authors to pursue future publications.</p>

<p align="left">Link to the submission site: Coming Soon</p>


<h2 align="center">Workshop Committee</h2>
<hr>

<p align="left"><strong>Workshop URL:</strong> https://ismart.ece.mcgill.ca/astad3/</p>

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

<h2 align="center">Workshop Poster</h2>
<hr>

<div class="row">
  <div class="col-sm-12">
    <h3 align="center">ASTAD3 Workshop Poster</h3>
    <div style="text-align: center; margin: 20px 0;">
      <img src="{{ site.url }}{{ site.baseurl }}/images/astad3.png" alt="ASTAD3 Workshop Poster" style="width: 100%; max-width: 800px; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
    </div>
  </div>
</div> 