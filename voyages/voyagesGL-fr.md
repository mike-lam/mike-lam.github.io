---  
layout: personal-fr  
title: Voyages 
description: Nos Voyages  
---  

<div>
<iframe src="https://www.google.com/maps/d/embed?mid=1_7c99T5F5ifV7p6hQWbARmetO9k" height="480" width="100%"></iframe>
<!-- 
to edit this map use 
https://www.google.com/maps/d/u/0/edit?mid=1_7c99T5F5ifV7p6hQWbARmetO9k&ll=49.389092877911395%2C-103.03218839375&z=5
and I think must be log as ****m4146**
-->
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
      <td>{{ post.date | date_to_string }}</td>
      <td><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></td>
      <td>{{ post.direction }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
