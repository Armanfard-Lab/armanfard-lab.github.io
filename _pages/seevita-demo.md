---
title: "SeeVita — Demo"
layout: page
excerpt: "Launch the SeeVita demo application"
permalink: /seevita/demo/
sitemap: true
---

### SeeVita Demo

Use the button below to launch the SeeVita demo application in a new tab.

{% if site.seevita_demo_url and site.seevita_demo_url != "" %}
<p>
  <a class="btn btn-primary" href="{{ site.seevita_demo_url }}" target="_blank" rel="noopener">Launch Demo</a>
  <a class="btn btn-default" href="{{ site.url }}{{ site.baseurl }}/seevita/">Back to SeeVita</a>
</p>
{% else %}
<div class="alert alert-warning" role="alert">
  The demo URL is not configured yet. Please provide a demo link so we can enable the launch button.
</div>
<p>
  <a class="btn btn-default" href="{{ site.url }}{{ site.baseurl }}/seevita/">Back to SeeVita</a>
</p>
{% endif %}


