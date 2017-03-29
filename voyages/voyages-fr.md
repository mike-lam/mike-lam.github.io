---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div id="mygeomap" class="wb-geomap position"	data-wb-geomap='{
		"tables": [{
			"id": "cities",
			"zoom": true,
			"tab": false,
			"popups": true,
			"visible": true,
			"popupsInfo": {
				"id": "citiesPopup",
				"height": 200,
				"width": 300,
				"close": true,
				"content": "<div style=\"white-space:nowrap;\"><p><strong>Census subdivision: </strong>_Census subdivision<div><a href=\"#\" class=\"button\" role=\"button\" title=\"Zoom to city\" aria-label=\"Zoom to city\" onclick=\"wb.doc.zoomFeature()\">Zoom to city</a></div></div>"
			},
			"style": {
				"type": "rule",
				"rule": [
				{
					"field": "Direction",
					"value": ["Ouest"],
					"filter": "EQUAL_TO",
					"init": {
						"strokeColor": "#0083f5",
						"fillColor": "#57a8f0",
						"pointRadius": 8,
						"fillOpacity": 0.80,
						"strokeWidth": 1.0
					}
				},
				{
					"field": "Direction",
					"value": ["Est"],
					"filter": "EQUAL_TO",
					"init": {
						"strokeColor": "#F90",
						"fillColor": "#F90",
						"pointRadius": 8,
						"fillOpacity": 0.80,
						"strokeWidth": 1.0
					}
				}
			]}
		}]
	}'>

  <div class="row">
    <div class="col-md-9">
      <div class="wb-geomap-map">
      </div>
  </div>
  <div class="row">
		<section>
			<div class="wb-geomap-layers col-md-12">
				<h3>Destinations</h3>
				<section>
					<h4>Villes</h4>
					<table id="cities" aria-label="Points" class="table wb-tables">
						<caption>
							Table of point geometries.
						</caption>
						<thead>
							<tr>
								<th>Direction</th>
								<th>Census subdivision</th>
							</tr>
						</thead>
						<tbody>
							<tr data-geometry="POINT (-79.3847, 43.6476)" data-type="wkt">
								<td>Ouest</td>
								<td><a href="http://www.wikipedia.org/wiki/Toronto" title="Toronto">Toronto</a></td>

							</tr>
							<tr data-geometry="POINT (-73.56123, 45.52927)" data-type="wkt">
								<td>Ouest</td>
								<td><a href="http://www.wikipedia.org/wiki/Montreal" title="Montreal">Montreal</a></td>
								
							</tr>
							<tr data-geometry="POINT (-114.05879, 51.04668)" data-type="wkt">
								<td>Est</td>
								<td><a href="http://www.wikipedia.org/wiki/Calgary" title="Calgary">Calgary</a></td>
								
							</tr>
							<tr data-geometry="POINT (-123.25825, 49.26047)" data-type="wkt">
								<td>Est</td>
								<td><a href="http://www.wikipedia.org/wiki/Vancouver" title="Calgary">Vancouver</a></td>
								
							</tr>
						</tbody>
					</table>
				</section>
			</div>

			
		</section>
	</div>
</div>


 Voyages dans l'ouest
 <ul class="posts">
   {% for post in site.categories.voyages %}
     <li><span>{{ post.date | date_to_string }}</span> Â» <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>{{ post.excerpt }}</li>
   {% endfor %}
 </ul>

