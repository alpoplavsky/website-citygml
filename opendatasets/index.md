---
layout: page
title:  Open data initiatives
permalink: /opendatasets/
---

# Open data initiatives

{% assign ds = site.data.opendatasets | sort: 'dataset' %}

<table class="table table-striped">

  <tr class="info">
    <td>dataset</td>
    <td>country</td>
    <td>year</td>
    <td>Building LOD</td>
    <td>other classes</td>
    <td>textures</td>
    <td>acquisition</td>
    <td>CityGML version</td>
    <td>notes</td>
  </tr>

  {% for i in ds %}
    <tr>
      <td><a href="{{ i.link }}">{{ i.dataset }}</a></td>
      <td>{{ i.country }}</td>
      <td>{{ i.year }}</td>
      <td>{{ i.building_lod }}</td>
      <td>{{ i.classes }}</td>
      <td>{{ i.texture }}</td>
      <td>{{ i.acquisition }}</td>
      <td>{{ i.version }}</td>
      <td>{{ i.notes }}</td>
    </tr>
  {% endfor %}

</table>
