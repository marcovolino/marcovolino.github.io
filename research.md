---
layout: default
---

<img src="/images/other/research.png" alt="" width="100%">


# Research
<div class="container" id="research">

<h3>Overview</h3>
<div class="container" id="overview">

<p>My research interests are at the intersection of computer vision, graphics and machine learning with a focus on visual media production. Below you can find: a list of projects and publications I have been involved in; funding I have recieved; and my service to the research community.</p>
</div>
<hr>

<h3>Projects</h3>
<div class="container" id="projects">
<table>
	<col width="150">
	<tbody>
		{% for project in site.projects reversed %}
		<tr>
			<td><img src="{{site.url}}/{{project.image}}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{project.title}}</b><br>
				<em>{{project.note}}</em><br>
					{{project.duration}}<br>
				<div class="btn-toolbar">
					{% for link in project.links %}
					<a class="btn btn-primary btn-xs" target="_blank" href="{{link.url}}">{{link.name}}</a>
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
<table>
	<col width="150">
	<tbody>
		{% for paper in site.publications reversed%}
		<tr>
			<td><img src="{{site.url}}/{{paper.image}}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{paper.title}}</b><br>
				<em>{{paper.authors}}</em><br>
					{{paper.venue}}<br>
					{{paper.year}}<br>
				<div class="btn-toolbar">
					{% for link in paper.links %}
					<a class="btn btn-primary btn-xs" target="_blank" href="{{link.url}}">{{link.name}}</a>
					{% endfor%}
			  </div>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>
</div>
<hr>



<h3>Service</h3>
<div class="container" id="publications">
<p>I have been involved in the organisation of the following conferences/meetings/workshops:</p>

<table>
	<col width="150">
	<tbody>
		{% for event in site.service reversed %}
		<tr>
			<td><img src="{{site.url}}/{{event.image}}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{event.title}}</b><br>
				<em>{{event.location}}</em><br>
					{{event.role}}<br>
				<div class="btn-toolbar">
					{% for link in event.links %}
					<a class="btn btn-primary btn-xs" target="_blank" 
					href="{{ link.url }}">{{ link.name }}</a>
					{% endfor%}
			  </div>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>
<br>

<p>I have served as a reviewer for the following conferences/journals/workshops:</p>
<ul>
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
