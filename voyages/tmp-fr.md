---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  


<div id="location_map"
	class="wb-geomap static"
	data-wb-geomap='{
		"tables": [{
			"id": "addNRCan",
			"style": {
				"type": "symbol",
				"init": {
					"pointRadius": 12,
					"graphicName": "star",
					"strokeColor": "#FF0000",
					"fillColor": "#FF0000",
					"fillOpacity": 0.7
				}
			}
		}]
	}'>
	<div class="row">
		<div class="col-md-4">
			<!-- Insert Map Start (mandatory) -->
			<div class="wb-geomap-map"></div>
			<!-- Insert Map End -->
		</div>
		<!-- Insert Layer Data Start (mandatory) -->
		<div class="wb-geomap-layers col-md-4">
			<table id="addNRCan" aria-label="NRCan Ottawa office adress" class="table">
				<caption class="wb-inv">Natural Resources Canada Ottawa office adress</caption>
				<thead>
					<tr>
						<th>Adress</th>
					</tr>
				</thead>
				<tbody>
					<tr data-geometry="POINT (-75.70535, 45.3995)" data-type="wkt">
						<td>615 Booth St.,<br />Ottawa (ON),<br />Canada,<br />K1A 0E8</td>
					</tr>
				</tbody>
			</table>
		</div>
		<!-- Insert Layer Data End -->
	</div>
</div>


 Voyages dans l'ouest
 <ul class="posts">
   {% for post in site.categories.voyages %}
     <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>{{ post.excerpt }}</li>
   {% endfor %}
 </ul>

