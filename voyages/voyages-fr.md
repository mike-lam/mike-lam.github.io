---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div id="mygeomap" class="wb-geomap static">
  <div class="row">
    <div class="col-md-9">
      <div class="wb-geomap-map">
      </div>
  </div>
<div class="row">
		<section>
			<div class="wb-geomap-layers col-md-12">
				<h3>Example - Inline Layer Data</h3>
				<p>Layers are created from the following tables. An attribute <em>data-geometry</em> to hold the geometry and an attribute <em>data-type</em> to hold the geometry type (wkt or bbox) are required for each row.</p>
				<section>
					<h4>Points</h4>
					<table id="cities" aria-label="Points" class="table wb-tables">
						<caption>
							Table of point geometries.
						</caption>
						<thead>
							<tr>
								<th>Rank</th>
								<th>Census subdivision</th>
								<th>Population 2011</th>
							</tr>
						</thead>
						<tbody>
							<tr data-geometry="POINT (-79.3847, 43.6476)" data-type="wkt">
								<td>1</td>
								<td><a href="http://www.wikipedia.org/wiki/Toronto" title="Toronto">Toronto</a></td>
								<td>2615060</td>
							</tr>
							<tr data-geometry="POINT (-73.56123, 45.52927)" data-type="wkt">
								<td>2</td>
								<td><a href="http://www.wikipedia.org/wiki/Montreal" title="Montreal">Montreal</a></td>
								<td>1649519</td>
							</tr>
							<tr data-geometry="POINT (-114.05879, 51.04668)" data-type="wkt">
								<td>3</td>
								<td><a href="http://www.wikipedia.org/wiki/Calgary" title="Calgary">Calgary</a></td>
								<td>1096833</td>
							</tr>
							<tr data-geometry="POINT (-75.68937, 45.41072)" data-type="wkt">
								<td>4</td>
								<td><a href="http://www.wikipedia.org/wiki/Ottawa" title="Ottawa">Ottawa</a></td>
								<td>883391</td>
							</tr>
							<tr data-geometry="POINT (-113.49590, 53.53398)" data-type="wkt">
								<td>5</td>
								<td><a href="http://www.wikipedia.org/wiki/Edmonton" title="Edmonton">Edmonton</a></td>
								<td>812201</td>
							</tr>
							<tr data-geometry="POINT (-79.65, 43.60)" data-type="wkt">
								<td>6</td>
								<td><a href="http://www.wikipedia.org/wiki/Mississauga" title="Mississauga">Mississauga</a></td>
								<td>713443</td>
							</tr>
							<tr data-geometry="POINT (-97.14352, 49.89375)" data-type="wkt">
								<td>7</td>
								<td><a href="http://www.wikipedia.org/wiki/Winnipeg" title="Winnipeg">Winnipeg</a></td>
								<td>663617</td>
							</tr>
							<tr data-geometry="POINT (-123.10091, 49.26428)" data-type="wkt">
								<td>8</td>
								<td><a href="http://www.wikipedia.org/wiki/Vancouver" title="Vancouver">Vancouver</a></td>
								<td>603502</td>
							</tr>
							<tr data-geometry="POINT (-79.76181, 43.68686)" data-type="wkt">
								<td>9</td>
								<td><a href="http://www.wikipedia.org/wiki/Brampton" title="Brampton">Brampton</a></td>
								<td>523911</td>
							</tr>
							<tr data-geometry="POINT (-79.86788, 43.25717)" data-type="wkt">
								<td>10</td>
								<td><a href="http://www.wikipedia.org/wiki/Hamilton,_Ontario" title="Hamilton, Ontario">Hamilton</a></td>
								<td>519949</td>
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
     <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>{{ post.excerpt }}</li>
   {% endfor %}
 </ul>

