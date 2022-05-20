---
layout: default
---


{% for paper in site.papers %}
	<h2>{{ paper.title }}</h2>
	<i>{{ paper.authors }}</i><br>
	<b>{{ paper.venue }} {{ paper.year }}</b>
	<p>{{ paper.content | markdownify }}</p>
{% endfor %}
