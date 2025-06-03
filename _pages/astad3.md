---
title: "ASTAD - NeurIPS 25"
layout: gridlay2
excerpt: "ASTAD - NeurIPS 25"
sitemap: false
permalink: /astad3/
---

<h1 align="center"> 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) </h1>

{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <div style="text-align: center; background: #000; display: inline-block; border-radius: 16px; padding: 16px; margin-bottom: 16px;">
    <img src="{{ site.url }}{{ site.baseurl }}/images/iSMART_white.png" align="middle" style="width: 250px; max-width: 90vw; height: auto; display: block; margin: 0 auto;" />
  </div>
  
  <h2 align="center">Overview</h2>
   <hr>
  <p align="center">The 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) aims to gather researchers and practitioners in AI to explore the latest advancements and novel approaches in anomaly detection using AI techniques, with a focus on spatial and temporal dimensions. As AI-assisted systems become more embedded in critical applications such as healthcare and industry, the demand for robust anomaly detection methods has intensified. Anomalies can significantly hinder system reliability, making robust detection methods critical for various real-world applications. In the age of foundation models and large models, the 3rd ASTAD workshop would incorporate discussion on the latest trends in anomaly detection, which includes foundation models in anomaly detection, zero-shot and few-shot anomaly detection, real-time anomaly detection in industrial automation and healthcare systems, and explainable AI methods that enhance transparency and reliability.</p>
 
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
    
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

</div>
{% endfor %}

<h2 align="center"> Call for Paper </h2>
<hr>
  
<p align="left">We invite researchers and practitioners to submit their original research contributions to the 3rd Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of NeurIPS 2025. This workshop aims to explore the latest advancements and novel approaches in anomaly detection using AI techniques within the domain of computer vision. Topics of Interest (but not limited to):</p>
  
  <ul>
    <li> Novel AI architectures for anomaly detection in images and videos </li>
    <li> Large-scale anomaly datasets and benchmarking methodologies </li>
    <li> Self-supervised, unsupervised, few-shot, and zero-shot anomaly detection techniques </li>
    <li> Continual learning for anomaly detection </li>
    <li> Foundation models and Large Models for anomaly detection </li>
    <li> Interpretability and explainability in anomaly detection </li>
    <li> Real-world anomaly detection applications in healthcare, industry, automotive sector, etc. </li>
    <li> Cross-modal and tabular anomaly detection </li>
    <li> Real-time anomaly detection </li>
  </ul>  

<p align="left">Submission Site: Coming Soon</p>

<h2 align="center"> Important Dates </h2>
<hr>

   <p align="left"> The important dates are as follows: </p>
<ul>
<li> <b>Paper submission deadline:</b> TBD </li>
 <li> <b>Author notification:</b> TBD </li>
 <li> <b>Camera-ready deadline:</b> TBD </li>
  </ul> 

  <h2 align="center"> Speakers </h2>
<hr>

<p align="center">To be announced</p>

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
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
    
  <p style="font-size:14px;">{{ member.bio }}</p>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
 <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>

{% assign number_printed = number_printed | plus: 1 %}

</div>
{% endif %}
{% endfor %}

{% for member in site.data.team_members %}
{% if member.name == "Hadi Hojjati" or member.name == "Thi Kieu Khanh Ho" or member.name == "Thomas Lai" or member.name == "Alexander Koran" or member.name == "Zihan Wang" or member.name == "Jack Wei" or member.name == "Sareh Soleimani" or member.name == "Navid Hassan Zadeh" or member.name == "Dimitrios Sinodinos" %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">
<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="25%" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
    
  <p style="font-size:14px;">{{ member.bio }}</p>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
 <a href="{{ member.scholar }}" target="_blank"><img src="https://user-images.githubusercontent.com/66117993/96351906-8c452000-1084-11eb-926f-6536bd0c6d57.png" alt="Google Scholar" style="width:26px;height:26px;margin:0px 3px"></a><a href="{{ member.linkedin }}" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width:26px;height:26px;margin:0px 3px"></a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
</div>
{% endif %}
{% endfor %} 