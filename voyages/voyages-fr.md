---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div id="mygeomap" class="wb-geomap position">
	<div class="row">
		<div class="col-md-9">
			<div class="wb-geomap-map"></div>
		</div>
{::comment}
		<-- Add optional map legend -->
		<div class="wb-geomap-legend col-md-3">
			<h2>Legend</h2>
			<-- Geomap will insert legend here -->
		</div>
{:/comment}
		<div class="row">
			<-- Add placeholder for overlays -->
			<div class="wb-geomap-layers col-md-12"></div>
		</div>
	</div>
</div>

 Voyages dans l'ouest
 <ul class="posts">
   {% for post in site.categories.voyages %}
     <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>{{ post.excerpt }}</li>
   {% endfor %}
 </ul>

