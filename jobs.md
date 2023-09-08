---
layout: default
---

<img src="/images/other/alive_banner.png" alt="" width="100%">

<h1>Current Openings</h1>
<div class="container" id="jobs-open">

{% capture now %}{{'now' | date: '%s' | plus: 0 %}}{% endcapture %}

{% for job in site.jobs %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 %}}{% endcapture %}
{% if date >= now %}
<h3><a href="{{job.url}}">{{job.title}}</a></h3>
{% endif %}
{% endfor %}
</div>

<h1>Previous Openings</h1>
<div class="container" id="jobs-closed">

{% for job in site.jobs %}
{% capture date %}{{job.expiryDate | date: '%s' | plus: 0 %}}{% endcapture %}
{% if date < now %}
<s><h3><a href="{{job.url}}">{{job.title}}</a></h3></s>
{% endif %}
{% endfor %}
</div>
