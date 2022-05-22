---
layout: default
---

## CV
<div class="container" id="cv">

<h3>Experience</h3>
<div class="container" id="experience">
<table>
	<col width="150">
	<tbody>
		{% for experience in site.experiences reversed %}
		<tr>
			<td><img src="{{site.url}}/{{experience.image}}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{experience.title}}</b><br>
				<em>{{experience.institute}}</em><br>
					{{experience.duration}}<br>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>

<h3>Education</h3>
<div class="container" id="education">
<table>
	<col width="150">
	<tbody>
		{% for experience in site.education reversed %}
		<tr>
			<td><img src="{{site.url}}/{{experience.image}}" alt="" width="100%" height="auto" /></td>
			<td>
				<b>{{experience.title}}</b><br>
				<em>{{experience.institute}}</em><br>
					{{experience.duration}}<br>
			</td>
		</tr>
		{% endfor %}
	</tbody>
</table>


For a detailed CV please contact me.
