---
title: "IJCAI-23 Tutorial"
layout: gridlay
excerpt: "IJCAI Tutorial"
sitemap: false
permalink: /ijcai23/
---

<h1 align="center">Tutorial: Deep Learning Methods for Unsupervised Time Series Anomaly Detection </h1>

{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <div style="text-align: center;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/ijcai-logo.png" align="middle">
</div>
  
  <h2 align="center">Abstract</h2>
   <hr>
  <p align="center">Time series anomaly detection (TSAD) is a crucial tool for detecting unusual patterns or outliers in large-scale time series datasets. With the increasing amount of data being generated in various industries, from financial transactions to industrial processes, it has become essential to identify anomalies that may indicate unusual events, fraud, or errors in the system. Deep learning algorithms have proven to be effective in detecting these anomalies, as they can learn complex patterns and relationships in the data that may not be apparent to humans. By detecting anomalies early, businesses can take proactive measures to prevent or minimize their impact, improving their overall performance and reducing risk. Thus, deep TSAD is an important tool for ensuring large-scale systems’ quality, reliability, and security and has attracted huge interest from the research community. This tutorial aims to provide the audience with a comprehensive and organized tutorial on state-of-the-art algorithms for time-series anomaly detection. We will first discuss the basic concepts of anomaly detection and time-series processing. Then, we will thoroughly review the deep learning methods for time-series anomaly detection, ranging from traditional autoencoder-based algorithms to the recently-proposed graph-based models. In the final parts of this tutorial, we will focus on some important considerations during the implementation, evaluation and dataset preparation for the deep time-series anomaly detection algorithms. Besides introducing the SOTA methods, this tutorial will aim to enable the researchers to apply them to solve real-world problems involving time series.</p>
 
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

<h2 align="center"> Location </h2>
<hr>
  
<p align="center"><b>To be Presented at:</b> IJCAI 2023</p>
  
<p align="center"><b>Date and Location:</b> August 20 PM, Macao, S.A.R</p>
  
 <p align="center"><b>Duration:</b> 2 Hours</p>

   
    
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



<h2 align="center"> Outline </h2>
<hr>
  <ul>
    <li>What is TSAD?</li>
    <li>Challenges in TSAD</li>
    <li>Some TSAD Applications</li>
    <li>Deep Learning and TSAD: A Tale of Triumph and Turmoil</li>
    <li>Deep Learning-based Methods</li>
    <li>Conclusion</li>
  </ul>  


  

