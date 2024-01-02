---
layout: single
title: Locations
permalink: /locations/
sidebar:
  nav: world-nav
toc: true
toc_label: "Contents"
toc_icon: "book"
---

## Aeros
<div id="map" style="width: 600px; height: 540px;"></div>
<script>
	var map = L.map('map', {
		crs: L.CRS.Simple,
		minZoom: -1,
		zoomAnimation: false
	});
	
	var bounds = [[0,0], [1080,1200]];
	var image = L.imageOverlay("/assets/images/terranea_with_labels_1.png", bounds).addTo(map)
	
	map.fitBounds(bounds);
	// map.setMaxBounds(bounds);
	
	var yx = L.latLng;

	var xy = function(x, y) {
		if (Array.isArray(x)) {    // When doing xy([x, y]);
			return yx(x[1], x[0]);
		}
		return yx(y, x);  // When doing xy(x, y);
	};
	
	//var hcoc = xy(618,1080-563);
	//L.marker(hcoc).addTo(map).bindPopup('Holy City of Caius');
	//var shelter1 = L.marker(hcoc);
	//var shelterMarkers = new L.FeatureGroup();
	
	//shelterMarkers.addLayer(shelter1).bindPopup('Holy City of Caius');
	
	//map.on('zoomend', function() {
	//	if (map.getZoom() < -0.1) {
	//		map.removeLayer(shelterMarkers);
	//	} else {
	//		map.addLayer(shelterMarkers);
	//	}
	//});
</script>

### Large Cities

#### Holy City of Caius

The capital of the Holy Republic of Caius, housing the headquarters of each government organization. The largest city on Aeros, only approximately 200,000 live within the city walls, but it houses nearly one million citizens in its extended territories. The Crucible floats directly above the city, connected magically by the Tower of Caius adjacent to the Grand Cathedral.

#### Geprusar

The capital of the Geprus province.

#### Port Revelry

A once large city nestled in the Geprusian Bay, it was razed by the titan [Jadwiga](/titans/#jadwiga) in SY 7659, leaving it in ruins. Since then, the city has wasted away, having been attacked by a titan twice in the last 200 years. 

Although still formally under the Church's purview, the city leadership is heavily influenced by a mafia-like group called *The Abandoned* that controls the city from the shadows. Two other organizations of note operate within the city: *The Crows*, a thieves guild that has many chapters spread across the large cities of Aeros, and *The Whispers*, a secretive group of information brokers that sell to the highest bidder.

[Hilda](/loc/npcs-main/#hilda-skyhelm) has numerous friends here - old pirates who have lost their crew - and recruits them to join the crew of the *Stormbreaker*.

### Small Cities & Towns

#### Ashborne

A small city in the Geprus province, it is named for the ash forest in which it resides. 

#### Jorren's Rest

A small village in the Geprus province mostly surrounded by wilderness. Hilda requested the party meet her here to join her crew.

#### Oldcrest

A tourist town adjacent to Dawnbringer Canyon, where the first Titan, [Gigas](/titans/#gigas), was slain.

### Places of Note

#### Redburn

Town where the first Titan, [Gigas](/titans/#gigas), appeared. Its ruins act as a reminder of the Titan's power.
