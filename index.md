---
layout: default
---

{% for paper in site.papers %}
<b><a href="{{ site.url }}{{ paper.url }}"> {{ paper.title }}  </a></b><br>
<i>{{ paper.authors }}</i> <br/>
<p>{{ paper.venue }} {{ paper.year }}</p>
<hr>
{% endfor %}
