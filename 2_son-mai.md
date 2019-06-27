---
layout: landing
title: Son mai
description: Bo suu tap tranh son mai.
image: assets/images/banner-01.jpg
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
	<div class="img_wrap">
		{% if image.path contains 'assets/images/fulls/son-mai' %}
		<a href="{{site.baseurl}}/assets/images/fulls/{{ image.name }}" class="portfolio-box">
		  <img src="{{site.baseurl}}/assets/images/thumbs/{{ image.name }}" class="image" >	
		</a>
		{% endif %}
	</div>
   {% endfor %}
</div>
</div>
</div>


<!-- <script src="{{site.baseurl}}/js/photo-grid.js"></script> -->
<script>
function getRandomSize(min, max) {
  return Math.round(Math.random() * (max - min) + min);
}
</script>
