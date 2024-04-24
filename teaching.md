---
layout: default
title: Teaching
---

<img src="/images/other/research.png" alt="" width="100%">

# Teaching 
I contribute to teaching in the school of <a href="https://www.surrey.ac.uk/school-computer-science-and-electronic-engineering" target="_blank">Computer Science and Electronic Engineering</a> (CSEE) on the undergraduate program in Electronic Engineering and Masters program in Artificial Inteligence. 


<h2>Current</h2>
<div class="container" id="current-teaching">
    {% for module in site.teaching reversed  %}
        {% if module.active == true %}
            <div>
                <h4><a href="{{module.module-url}}" target="_blank">{{ module.title }} ({{module.code}})</a></h4>
                <b>Role:</b> {{module.role}} <br>
                <b>Duration:</b> {{module.duration}} <br>
                <b>Description:</b> {{ module.content | markdownify }}
            </div>
            <br>
        {% endif %}
    {% endfor %}
</div>


<h2>Previous</h2>
<div class="container" id="previous-teaching">
    {% for module in site.teaching reversed  %}
        {% if module.active == false %}
            <div>
                <h4><a href="{{module.module-url}}" target="_blank">{{ module.title }} ({{module.code}})</a></h4>
                <b>Role:</b> {{module.role}} <br>
                <b>Duration:</b> {{module.duration}} <br>
                <b>Description:</b> {{ module.content | markdownify }} 
            </div>
            <br>
        {% endif %}
    {% endfor %}
</div>
