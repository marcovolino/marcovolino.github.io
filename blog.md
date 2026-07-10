---
layout: default
title: Blog
description: Blog posts and notes from Marco Volino on computer vision, computer graphics, visual media production and academic research.
image: /images/cv/marco.jpg
---


<h2>Blog</h2>

<div>
{% for post in site.blog reversed %}
    
    <h4> <a href="{{ post.url }}">{{ post.title }}</a> </h4>
    
{% endfor %}


</div>
