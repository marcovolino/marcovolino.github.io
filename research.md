---
layout: default
title: Research
description: Research projects, publications, collaborators and community service in computer vision, graphics, digital humans, volumetric video, neural rendering and immersive media.
image: /images/other/research.png
---

<img src="{{ '/images/other/research.png' | relative_url }}" alt="" width="100%">


# Research
<div class="container" id="research">

<h3>Overview</h3>
<div class="container" id="overview">

<p>My research interests are at the intersection of computer vision, graphics and machine learning with a focus on visual media production and immersive technology. Below you can find: (i) a list of projects, funding and publications I have been involved in; people I have worked with; and my service to the research community.</p>
</div>
<hr>

<h3>Projects</h3>
<div class="container" id="projects">
<table class="media-list">
	<col width="150">
	<tbody>
		{% for project in site.projects reversed %}
		<tr>
			<td><img src="{{ project.image | prepend: '/' | relative_url }}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{project.title}}</b><br>
				<em>{{project.note}}</em><br>
					{{project.duration}}<br>
				<div class="btn-toolbar">
					{% for link in project.links %}
					<a class="btn btn-primary btn-xs" target="_blank" rel="noopener" href="{{link.url}}">{{link.name}}</a>
					{% endfor%}
			  </div>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>
<hr>

<h3>Publications</h3>
<div class="container" id="publications">
<table class="media-list publication-list">
	<col width="150">
	<tbody>
    {% assign papers_by_year = site.publications | reverse %}
    {% for paper in papers_by_year %}
    <tr>
        <td><img src="{{ paper.image | prepend: '/' | relative_url }}" alt="" width="100%" height="auto" /></td>
        <td>
            <b>{{paper.title}}</b><br>
            <em>{{paper.authors}}</em><br>
                {{paper.venue}}<br>
                {{paper.year}}<br>
            <div class="btn-toolbar">
                {% for link in paper.links %}
                    {% assign url = link.url %}
                    {% if url contains '://' %}
                        <a class="btn btn-primary btn-xs" target="_blank" rel="noopener" href="{{link.url}}">{{link.name}}</a>
                    {% else %}
                        <a class="btn btn-primary btn-xs" target="_blank" rel="noopener" href="{{ link.url | prepend: '/' | relative_url }}">{{link.name}}</a>
                    {% endif %}
                {% endfor %}
                {% if paper.headline %}<b class="highlight btn btn-primary btn-xs "> {{ paper.headline}} </b>{% endif %}
          </div>
        </td>
    </tr>
            {% endfor %}
	</tbody>
</table>
</div>
<hr>

<h3>Team</h3>
<div class="container" id="team">
    <p> I have been fortunate enough to work with the following people:</p>
    <table class="team-list">
        <tbody>
            {% assign people_sorted = site.team | sort: "duration"%}
            {% for people in people_sorted reversed %}
            <tr>
                <td>
                {% if people.linkedin %}
                    <b><a href="{{people.linkedin}}" target="_blank" rel="noopener">{{people.name}}</a></b>
                {% else %}
                <b>{{people.name}}</b>
                {% endif %}
                </td>
            <td>
                <p>{{people.duration}}</p>
            </td>
            </tr>
            <tr>
                <td>
                <p><em>Position: {{people.position}}</em></p>
                {% if people.thesis-url %}
                    <p><em>Topic: <a href="{{people.thesis-url}}" target="_blank" rel="noopener">{{people.topic}}</a></em></p>
                {% else %}
                    <p><em>Topic: {{people.topic}}</em></p>
                {% endif %}
                </td>
            </tr>
            {% endfor %}
        </tbody>
    </table>    
</div>
<hr>



<h3>Service</h3>
<div class="container" id="service">
<p>I have been involved in the organisation of the following conferences/meetings/workshops:</p>

<table class="media-list service-list">
	<col width="150">
	<tbody>
		{% for event in site.service reversed %}
		<tr>
			<td><img src="{{ event.image | prepend: '/' | relative_url }}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{event.title}}</b><br>
				<em>{{event.location}}</em><br>
					{{event.role}}<br>
				<div class="btn-toolbar">
					{% for link in event.links %}
					<a class="btn btn-primary btn-xs" target="_blank" rel="noopener" 
					href="{{ link.url }}">{{ link.name }}</a>
					{% endfor%}
			  </div>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>
<br>

<p>I have served as a reviewer for the following funders/conferences/journals/workshops:</p>
    <ul>
        <li>Swiss National Science Foundation</li>
        <li>ACM Transactions on Graphics (TOG)</li>
        <li>IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)</li>
        <li>IEEE/CVF International Conference on Computer Vision (ICCV)</li>
        <li>European Conference on Computer Vision (ECCV)</li>
        <li>International Conference on 3D Vision (3DV)</li>
        <li>ACM SIGGRAPH European Conference on Visual Media Production(CVMP)</li>
        <li>British Machine Vision Conference (BMVC)</li>
        <li>Virtual Reality & Intelligent Hardware (VRIH)</li>
        <li>Multimedia Systems (MMSJ)</li>
        <li>Computer Vision and Image Understanding (CVIU)</li>
        <li>IET Computer Vision</li>
        <li>3D Reconstruction in the Wild (3DRW)</li>
    </ul>
</div>
<hr>

</div>
