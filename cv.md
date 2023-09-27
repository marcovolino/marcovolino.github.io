---
layout: default
---

<h2>Marco Volino</h2>
<b>PhD, MEng</b>

<div class="container" id="cv">

<!------------------------------------------------------>
<h3>Profile</h3>
<div class="container" id="profile">
With over 10 years of experience in research and development, Marco Volino is a passionate research scientist and engineer with expertise at the intersection of computer vision, computer graphics and machine learning.
To date, Marco’s work has focused on advancing the capabilities of digital content production in collaboration with creative industry partners to facilitate high-quality immersive audio-visual media experiences. 
Marco’s work has primarily addressed challenges related to camera calibration, 3D reconstruction, pose estimation, animation, rendering, and immersive technology, such as virtual and augmented reality (AR/VR). 
Marco has significant experience in both hardware and software development, having designed, developed and deployed a range of synchronised camera systems, and is highly proficient in a number of programming  languages, APIs, and development and software tools.
</div>

<!------------------------------------------------------>
<h3>Skills</h3>
<div class="container" id="skills">

<table>
{% for section in site.data.cv_skills %}

<tr>
    <td><b>{{ section.title }}</b></td>
    <td>
{% for skill in section.nested %}
   {% if skill.url != "" %}
        <a href="{{skill.url}}" target="_blank">{{ skill.title}}</a>
    {% else %}
        {{ skill.title}}
   {% endif %}
    &ensp;
{% endfor %}
    </td>
  </tr>
{% endfor %}
</table>
</div>

<!------------------------------------------------------>
<h3>Experience</h3>
<div class="container" id="experience">
<table>
    <col style="width:80%">
    <col style="width:20%">
	<tbody>
		{% for experience in site.experiences reversed %}
		<tr>
			<td>
				<span class="left"><b>{{experience.title}}</b></span><br>
				{{experience.institute}}<br>
                <em>{{experience.duration}}</em><br>
                {{ experience.content | markdownify }}
			</td>
            <td valign="top"><img src="{{site.url}}/{{experience.image}}" alt="" width="80px" height="auto" /></td>         
		</tr>
		{% endfor %}
	</tbody>
</table>
</div>


<!------------------------------------------------------>
<h3>Education</h3>
<div class="container" id="education">
<table>
    <col style="width:80%">
    <col style="width:20%">
    <tbody>
        {% for experience in site.education reversed %}
        <tr>
            <td>
                <span class="left"><b>{{experience.title}}</b></span><br>
                {{experience.institute}}<br>
                <em>{{experience.duration}}</em><br>
                {{ experience.content | markdownify }}
            </td>
            <td valign="top"><img src="{{site.url}}/{{experience.image}}" alt="" width="80px" height="auto" /></td>         
        </tr>
        {% endfor %}
    </tbody>
</table>
</div>


</div>
