---
layout: default
---


<h2>Blog</h2>

<div>
{% for post in site.blog reversed %}
    
    <h4> <a href="{{ post.url }}">{{ post.title }}</a> </h4>
    
{% endfor %}


</div>
