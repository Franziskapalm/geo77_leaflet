# geo77_leaflet
 A simple web map with earthquakes in Germany

<!DOCTYPE html>
<html lang="en">
<head>
 <!-- set the charset -->
 <meta charset="utf-8">
 <!-- set make the map responsive -->
 <meta http-equiv="X-UA-Compatible" content="IE=edge">
 <meta name="viewport" content="initial-scale=1,user-scalable=no,maximum-scale=1,width=device-width">
 <meta name="mobile-web-app-capable" content="yes">
 <meta name="apple-mobile-web-app-capable" content="yes">
  <!-- set the title shown in the browser tab -->
 <title>Earthquake Map</title>
  <!-- Links to the leaflet CSS and JS -->
 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
 <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>
  <!-- styles for elements html and body: fullscreen  -->
 <style>
  html, body {
 	 width: 100%;
     height: 100%;
	 padding: 0;
	 margin: 0;
  }
 </style>	
</head>
<body>
 <!-- set the div element containing the map -->
 <div id="mapid" style="width: 100%; height: 100%; padding: 0; margin: 0;"></div>
 
 
 <script>
 
  // Create Leaflet map
  var mymap = L.map('mapid').setView([51.5, 11.5], 6);
 
  // Add basemaps
  // basemap 1:
  var osm_basemap = L.tileLayer('https://{s}.tile.openstreetmap.de/tiles/osmde/{z}/{x}/{y}.png', {
	  attribution: '<a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
  }).addTo(mymap);
 </script>
 
</body>
</html>
