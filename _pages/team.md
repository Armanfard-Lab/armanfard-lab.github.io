---
title: "iSMART Lab - Team"
layout: gridlay
excerpt: "Team members"
sitemap: false
permalink: /team/
---

<h2 align="center"> Founder and Director </h2>

{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-circle" width="25%" style="display: block; margin-left: auto; margin-right: auto;aspect-ratio: 1; border-radius:50%"/>
  <h3 align="center">{{ member.name }}</h3>
  <p align="center"><i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> --></p>
    
  <p align="center">Dr. Armanfard is the founder and principal investigator of the iSMART Lab. She holds the position of Associate Professor (tenured) in the Department of Electrical and Computer Engineering at McGill University, as well as at Mila - Quebec AI Institute. She is also affiliated with McGill Centre for Intelligent Machines (CIM), McGill initiative in Computational Medicine (MiCM), and McGill Institute for Aerospace Engineering (MIAE). She earned her Ph.D. and Postdoctoral in Artificial Intelligence from McMaster University and the University of Toronto in Canada. Her contributions to the field of AI have been acknowledged through numerous awards from institutions, including the Natural Sciences and Engineering Research Council of Canada, AgeWell, Vanier-Banting, the Fonds de recherche du Québec, McMaster University, McGill University, the University of Toronto, the Canadian Institutes of Health Research, Scale AI, National Research Council Canada, and Canada Foundation for Innovation, among others. Narges's academic accomplishments extend to the publication of over fifty AI-focused articles across distinguished platforms, including AAAI, WACV, ECAI, BMVC, ECML PKDD, TPAMI, TNNLS, TSMC, TIFS, and more.</p>
 
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
  <center>
  <a href="https://scholar.google.com/citations?user=V8pn4tIAAAAJ&hl=en" target="_blank"><img src="https://raw.githubusercontent.com/Armanfard-Lab/armanfard-lab.github.io/gh-pages/images/google-scholar-square.png" alt="Google Scholar" style="aspect-ratio: 1;width:26px;height:26px;margin:0px 3px"></a><a href="https://ca.linkedin.com/in/armanfardn" target="_blank"><img src="https://github.com/Armanfard-Lab/armanfard-lab.github.io/blob/gh-pages/images/new-linkedin-logo-white-black-png.png?raw=true" alt="LinkedIn" style="aspect-ratio: 1;width:26px;height:26px;margin:0px 3px"></a>
  </center>
</div>

{% assign number_printed = number_printed | plus: 1 %}

</div>
{% endfor %}


<h2 align="center"> Research Team Members </h2>

{% assign number_printed = 0 %}
{% for member in site.data.postdoc %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="18%" style="aspect-ratio: 1; border-radius:50%;float: left" />
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
</div>

{% assign number_printed = number_printed | plus: 1 %}
  
</div>

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}


{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="rounded-circle" width="18%" style="aspect-ratio: 1; border-radius:50%;float: left" />
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




{% assign number_printed = 0 %}
{% for member in site.data.bsc %}

{% assign even_odd = number_printed | modulo: 2 %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="18%" class="rounded-circle" style="aspect-ratio: 1; border-radius:50%;float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
    
  <p style="font-size:14px;">{{ member.project }}</p>
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



<h2 align="center"> Alumni </h2>
<div class="row">

<div class="col-sm-12 clearfix">
<h4>Graduate Researchers</h4>
{% for member in site.data.alumni_members %}
{{ member.name }}<br>
<i>{{ member.duration }}</i>
{% endfor %}
</div>

<div class="col-sm-12 clearfix">
<h4>Undergraduate Reserachers</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}<br>
<i>{{ member.duration }}</i>
{% endfor %}
</div>



</div>
  

