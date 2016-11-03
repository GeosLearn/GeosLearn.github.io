---
title: Mapping resources
featured: images/pic4.jpg
layout: post
---

Global distribution of mineral & oil resources and reserves are essential to understand not only the economic wealth of specific countries but also some of the major conflicts taking place in different regions of the World.
Australia has an abundant and diverse range of energy resources. It has very large coal resources that underpin exports and low-cost domestic electricity production, more than one third of the world's known uranium resources, and substantial conventional gas and coal seam gas resources.

<head>
   <link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.5/leaflet.css" />
   <script src="http://cdn.leafletjs.com/leaflet-0.5/leaflet.js"></script>
</head>
<div class="col-md-6" id="map" style="width:100%; height:400px"></div>
<script>
  var map = L.map('map').setView([-20.7353, 116.8458], 8);
  L.tileLayer('http://{s}.tile.stamen.com/terrain/{z}/{x}/{y}.jpg', {
      maxZoom: 18,
      attribution: 'Map tiles by <a href="http://stamen.com">Stamen Design</a>, under <a href="http://creativecommons.org/licenses/by/3.0">CC BY 3.0</a>. Data by <a href="http://openstreetmap.org">OpenStreetMap</a>, under <a href="http://creativecommons.org/licenses/by-sa/3.0">CC BY SA</a>.'
  }).addTo(map);
  var marker_1 = L.marker([-20.7353, 116.8458]);
  marker_1.bindPopup("Karratha Gas Plant (Woodside)");
  map.addLayer(marker_1)
</script>
**Mapping these resources are essential skills for geoscientists. Using open-source libraries, you will learn how to map some of Australian offshore resources with Jupyter notebooks.**

<section>
  <header>
    <span class="byline"><font color = "#000000">Preamble</font></span>
  </header>
  <p>TODO</p>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Lecture Material</font></span>
  </header>
  <p>TODO</p>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">For the labs</font></span>
  </header>
  <p>TODO</p>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Going further</font></span>
  </header>
  <p>TODO</p>
</section>
