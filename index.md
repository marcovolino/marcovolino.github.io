---
layout: default
---

<!-- BIO SECTION -->
<div class="container" id="bio">

	<!-- BIO IMAGE -->
	<div id="bio_image">
		<img class="img-circle" id="profile" src="images/cv/marco.jpg" alt="marco" hspace="20" width="150" height="150">
	</div>
	
	<!-- BIO TEXT -->
	<div id="bio_text">
		<p>
			I am currently a <b>Lecturer in Computer Vision and Graphics</b> in the <a target="_blank" href="https://www.surrey.ac.uk/centre-vision-speech-signal-processing"><b>Centre for Vision, Speech and Signal Processing</b></a> at the <a target="_blank" href="https://www.surrey.ac.uk/"><b>University of Surrey</b></a>. I am interested in using computer vision and graphics techniques to facilitate volumetric video capture, reconstruction, editing and rendering from multiple camera systems for applications in film, broadcast and gaming. I also have a keen interest in <a target="_blank" href="https://500px.com/marcovolino"><b>Photography</b></a>.
		</p>
		<p>
			In 2016, I received a PhD from the University of Surrey supervised by <a target="_blank" href="http://cvssp.org/Personal/AdrianHilton/Welcome.html"><b>Prof. Adrian Hilton</b></a> and <a target="_blank" href="http://www.bbc.co.uk/rd/people/g-a-thomas" ><b>Prof. Graham Thomas</b></a> (BBC R&amp;D). My PhD introduced novel techniques to compactly represent multiple view video to allow efficient free-viewpoint rendering. During this time, I undertook an internship at the <a target="_blank" href="http://ict.usc.edu/"><b>University of Southern California, Institute for Creative Technologies</b></a> where I designed and built a photogrammetry scanning cage for rapid avatar creation, and a three month internship at <a target="_blank" href="http://www.bbc.co.uk/rd"><b>BBC R&amp;D</b></a> integrating my PhD research into a WebGL-based renderer.
		</p>
		<p>
			In 2011, I obtained an <a target="_blank" href="https://www.surrey.ac.uk/undergraduate/electrical-and-electronic-engineering"><b>MEng in Electronic Engineering</b></a> <b>(Distinction)</b> at the University of Surrey during which I spent a professional training year at <a target="_blank" href="https://www.sony.co.uk/pro/products/solutions-broadcast"><b>Sony Broadcast and Professional Research Labs</b></a> and a three month summer internship at the <a target="_blank" href="http://www.isr.reading.ac.uk/"><b>Intelligent Systems Research Laboratory University of Reading</b></a>.
		</p>
		<br>
	</div>
</div>
<hr>

## News 
<div class="container" id="news">
{% for article in site.news reversed %}
<ul>
<li><b>{{article.date | date: "%Y/%m" }}</b> - {{article.title}}</li>
</ul>
{% endfor %}
</div>
<hr>
