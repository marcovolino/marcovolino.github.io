---
layout: default
---

{% for paper in site.papers %}
<h3><a href="{{ site.url }}{{ paper.url }}"> {{ paper.title }}  </a></h3>
<i>{{ paper.authors }}</i> <br/>
<p>{{ paper.venue }} {{ paper.year }}</p>
<hr>
{% endfor %}
