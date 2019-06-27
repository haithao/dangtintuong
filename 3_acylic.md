---
title: ACRYLIC
layout: landing
description: Bo suu tap tranh acrylic.
image: assets/images/banner-long.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<style>
.container-fluid {
    padding-right: 1px;
    padding-left: 1px;
    margin-right: auto;
    margin-left: auto;
}
</style>

<section id="photos">
<div class="container-fluid">
<div class="row-no-gutters">
	{% assign image_files = site.static_files | where: "image", true %}
	{% for image in image_files %}
	{% if image.path contains 'fulls/Acrylic' %}
	<div class="img_wrap">		
		<a href="{{site.baseurl}}/assets/images/fulls/{{ image.name }}" class="portfolio-box">
		  <img src="{{site.baseurl}}/assets/images/thumbs/{{ image.name }}" class="image" >	
		</a>		
	</div>
	{% endif %}
    {% endfor %}
</div>
</div>
</section>
</div>


<!-- <script src="{{site.baseurl}}/js/photo-grid.js"></script> -->
<script>
function getRandomSize(min, max) {
  return Math.round(Math.random() * (max - min) + min);
}
</script>