---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div>
<iframe src="https://www.google.com/maps/d/embed?mid=1_7c99T5F5ifV7p6hQWbARmetO9k" height="480" width="100%"></iframe>
</div>

<table class="wb-tables table table-striped table-hover" data-wb-tables='{ "paging" : false }'>
  <thead>
    <tr>
      <th>Date</th>
      <th>Ville</th>
      <th>Direction</th>
    </tr>
  </thead>
  <tbody>
  {% for post in site.categories.voyages %}
    <tr>
      <td>{{ post.date }}</td>
      <td><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></td>
      <td>DirectionXXX</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
