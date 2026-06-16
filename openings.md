---
layout: default
---

<img src="/images/other/alive_banner.png" alt="" width="100%">

<h2>Current</h2>
<div class="container" id="jobs-open">

{% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
{% assign current_openings_count = 0 %}

{% for job in site.openings %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 }}{% endcapture %}
{% if date >= now %}
{% assign current_openings_count = current_openings_count | plus: 1 %}
<h4><a href="{{job.url}}">{{job.title}}</a></h4>
{% endif %}
{% endfor %}
{% if current_openings_count == 0 %}
<p><em>No current openings</em></p>
{% endif %}
</div>

<h2>Previous</h2>
<div class="container" id="jobs-closed">

{% for job in site.openings reversed%}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 }}{% endcapture %}
{% if date < now %}
<s><h4><a href="{{job.url}}">{{job.title}}</a></h4></s>
{% endif %}
{% endfor %}
</div>
