---
title: "ASTAD - WACV 24"
layout: gridlay2
excerpt: "ASTAD - WACV 24"
sitemap: false
permalink: /wacv24/
---

<h1 align="center"> 1st Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD) </h1>

{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <div style="text-align: center;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/WACV.png" align="middle" style="max-width: 100%;">
</div>
  
  <h2 align="center">Overview</h2>
   <hr>
  <p align="center">Anomalies and outliers in visual data can significantly impact the performance and reliability of computer vision systems. As the applications of computer vision continue to grow across various domains, the need for robust and efficient anomaly detection techniques becomes paramount. This workshop aims to bring together researchers, industry experts, and practitioners to explore the latest advancements in automated anomaly detection methods specifically tailored for computer vision tasks. The primary objective of this workshop is to provide a platform for researchers to share and discuss their cutting-edge research in the field of anomaly detection in computer vision. We seek to foster collaboration, encourage knowledge exchange, and promote the development of novel approaches to tackle the challenges posed by anomalies in visual data. The expected outcome of this workshop is to foster a vibrant exchange of knowledge and ideas among researchers and practitioners in the field. Through insightful presentations, discussions, and interactive sessions, participants will gain a comprehensive understanding of cutting-edge AI-based methodologies for anomaly detection in computer vision. The workshop aims to encourage collaborations, inspire new research directions, and promote the development of innovative solutions to address real-world challenges in anomaly detection. As a result, attendees will leave the workshop equipped with valuable insights and practical tools that will contribute to advancements in anomaly detection techniques, ultimately leading to more robust and reliable computer vision systems across various domains.</p>
 
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
  
<p align="left">We invite researchers and practitioners to submit their original research contributions to the 1st Workshop on Automated Spatial and Temporal Anomaly Detection (ASTAD), held as part of WACV 2024. This workshop aims to explore the latest advancements and novel approaches in anomaly detection using AI techniques within the domain of computer vision. Topics of Interest (but not limited to):</p>
  
  <ul>
    <li> Novel AI architectures for anomaly detection in images and videos </li>
    <li> Large-scale anomaly datasets and benchmarking methodologies </li>
    <li> Self-supervised, unsupervised, and few-shot anomaly detection techniques </li>
    <li> Continual Learning for anomaly detection </li>
    <li> Interpretability and explainability in anomaly detection models </li>
    <li> Real-world applications of anomaly detection in computer vision </li>
  </ul>  

<p align="left">Submission Site: <a href="https://cmt3.research.microsoft.com/ASTAD2024">Microsoft CMT</a></p>


<h2 align="center"> Schedule </h2>
<hr>

Jan. 08, 2024 (Time below is in Hawaii local time)
  
  
  <ul>
    <li>  8:20-8:30 AM: <b>Opening</b> </li>
    <li>  8:30-9:30 AM: <b>Keynote Talk by Prof. Ye Zhu</b> </li>
    <li> 9:30-10:30 AM: <b>Keynote Talk by Prof. Jie Rien</b>  </li>
    <li> 10:30-10:40 AM: <b>Break</b>  </li>
    <li> 10:40-11:00 AM: <b>Oral Presentation Session</b>  </li>
    <li> 11:00-11:30 PM: <b> Keynote Take by Pemula Latha</b>  </li>
    <li> 11:30-12:30 PM: <b> Keynote Talk by Prof. Jaemin Yoo</b>  </li>
  </ul>  


 
<h2 align="center"> Important Dates </h2>
<hr>

   <p align="left"> The important dates are as follows: </p>
<ul>
<li> <b>Paper submission deadline:</b> Oct 25, 2023 </li>
 <li> <b>Author notification:</b> Nov 14, 2023 </li>
 <li> <b>Camera-ready deadline:</b> Nov 19, 2023 </li>
  </ul> 

  <h2 align="center"> Speakers </h2>
<hr>

{% assign number_printed = 0 %}
{% for member in site.data.wacvspeak %}

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

{% endfor %}

    
<h2 align="center"> Organizers </h2>
<hr>
{% assign number_printed = 0 %}
{% for member in site.data.wacv24member %}

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

{% endfor %}



  

