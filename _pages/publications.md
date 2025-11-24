---
title: "iSMART Lab - Publications"
layout: gridlay
excerpt: "iSMART Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

## Group highlights

(For full list of publications and patents see <a href="https://scholar.google.com/citations?hl=en&user=V8pn4tIAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a>)

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

<div class="row">

 <div class="col-sm-12 clearfix">
  <div class="well">
   <pubtit>{{ publi.title }}</pubtit>
   <div style="display: flex; gap: 16px; align-items: flex-start;">
     <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" style="width: 25%; height: 180px; object-fit: cover;" />
     <div style="flex: 1;">
       <p>{{ publi.description }}</p>
       <p><em>{{ publi.authors }}</em></p>
       <p><strong><a href="{{ publi.link.url }}" target="_blank">{{ publi.link.display }}</a></strong></p>
       <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
       <p> {{ publi.news2 }}</p>
     </div>
   </div>
  </div>
 </div>

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
{% endif %}

<p> &nbsp; </p>



