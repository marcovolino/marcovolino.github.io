---
layout: default
title: Home
seo_title: Marco Volino | Computer Vision and Graphics
description: Marco Volino researches computer vision, graphics and machine learning for digital humans, volumetric video, neural rendering and immersive media.
image: /images/cv/marco.jpg
---

<!-- BIO SECTION -->
<div class="container" id="bio">

	<!-- BIO IMAGE -->
	<div id="bio_image">
		<img class="img-circle" id="profile" src="images/cv/marco.jpg" alt="marco" hspace="20" width="150" height="150">
	</div>
	
	<!-- BIO TEXT -->
	<div id="bio_text">
		<h1>Marco Volino</h1>
		<p class="lead">
			Senior Lecturer in Computer Vision and Graphics at the University of Surrey, working on visual computing for digital humans, volumetric video, neural rendering and immersive media production.
		</p>
		<p>
			Marco is based in the <a href="https://www.surrey.ac.uk/centre-vision-speech-signal-processing" target="_blank" rel="noopener">Centre for Vision, Speech and Signal Processing</a> and is a Principal AI Fellow at the <a href="https://www.surrey.ac.uk/ai" target="_blank" rel="noopener">Surrey Institute for People-Centred AI</a>. His research bridges computer vision, computer graphics and machine learning for creative industry applications across film, broadcast, games, virtual production and extended reality.
		</p>
		<p>
			He has contributed to research and innovation projects with creative and technology partners including BBC Research & Development, Epic Games, Humain Studios, Foundry, Figment Productions and the CoSTAR National Lab, translating work in multi-camera capture, 4D human performance capture, neural rendering and AI-enabled media tools into production-facing systems.
		</p>
		<p>
			His <a href="{{ '/research/#publications' | relative_url }}">publications</a> span leading venues in computer vision, graphics and immersive media, including CVPR, ECCV, ICCV, 3DV and IEEE VR. Alongside research, Marco <a href="{{ '/teaching/' | relative_url }}">teaches visual computing</a> and contributes to the research community through roles including CVMP Conference Co-Chair, CVMP Steering Committee member, BMVC Area Chair and DynaVis workshop co-organiser.
		</p>
		<div class="homepage-actions">
			<a class="btn btn-primary btn-sm" href="{{ '/research/' | relative_url }}">Research</a>
			<a class="btn btn-primary btn-sm" href="{{ '/research/#publications' | relative_url }}">Publications</a>
			<a class="btn btn-primary btn-sm" href="{{ '/teaching/' | relative_url }}">Teaching</a>
			<a class="btn btn-primary btn-sm" href="{{ '/openings/' | relative_url }}">Openings</a>
		</div>
	</div>
</div>

<hr>

<h2 id="news">News</h2>
<div class="container news-list">
	<ul>
{% for article in site.news reversed %}
		<li><b>{{article.date | date: "%Y/%m" }}</b> - {{article.title}}</li>
{% endfor %}
	</ul>
</div>
<hr>
