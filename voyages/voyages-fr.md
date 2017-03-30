---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div id="mygeomap" class="wb-geomap position"  data-wb-geomap='{
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
        "content": "<div style=\"white-space:nowrap;\"><p><strong>Ville: </strong>_Ville<div><a href=\"#_Ville\" class=\"button\" role=\"button\" title=\"Zoom a la ville\" aria-label=\"Zoom a la ville\" onclick=\"wb.doc.zoomFeature()\">Zoom a la ville</a></div></div>"
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
                <th>Ville</th>
              </tr>
            </thead>
            <tbody>
              {% for post in site.categories.voyages %}
                <tr data-geometry="{{ post.point }}" data-type="wkt">
                  <td>Ouest</td>
                  <td><a href="{{ post.url }}" title="{{ post.title }}" id="{{ post.title }}">{{ post.title }}</a></td>
                </tr>
              {% endfor %}
            </tbody>
          </table>
        </section>
      </div>
    </section>
  </div>
</div>
