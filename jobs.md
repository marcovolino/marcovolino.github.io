---
layout: default
---

<img src="/images/other/alive_banner.png" alt="" width="100%">

<h2>Current Openings</h2>
<div class="container" id="jobs-open">

{% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}

{% for job in site.jobs %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 }}{% endcapture %}
{% if date >= now %}
<h4><a href="{{job.url}}">{{job.title}}</a></h4>
{% endif %}
{% endfor %}
</div>

<h2>Previous Openings</h2>
<div class="container" id="jobs-closed">

{% for job in site.jobs %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 }}{% endcapture %}
{% if date < now %}
<s><h4><a href="{{job.url}}">{{job.title}}</a></h4></s>
{% endif %}
{% endfor %}
</div>
