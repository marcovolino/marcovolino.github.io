---
layout: default
---

<img src="/images/other/alive_banner.png" alt="" width="100%">

<h2>Current</h2>
<div class="container" id="jobs-open">

{% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}

{% for job in site.openings %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 }}{% endcapture %}
{% if date >= now %}
<h4><a href="{{job.url}}">{{job.title}}</a></h4>
{% endif %}
{% endfor %}
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
