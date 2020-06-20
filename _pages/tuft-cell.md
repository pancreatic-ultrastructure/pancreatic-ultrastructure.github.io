---
title: Tuft cell
layout: post
---

<link rel="stylesheet" href="https://pancreatic-ultrastructure.github.io/css/leaflet.css" />
<!--[if lte IE 8]>
        <link rel="stylesheet" href="css/leaflet.ie.css" />
    <![endif]-->
<style type="text/css">
        #photo {
            width: 800px;
            height: 800px;
            padding: 0;
            margin: 0;
        }
</style>

<div id="photo"></div>
<script src="https://pancreatic-ultrastructure.github.io/js/leaflet.js"></script>
<script type="text/javascript" src="https://pancreatic-ultrastructure.github.io/js/L.TileLayer.Zoomify.js"></script>  
<script type="text/javascript">
var map = L.map('photo').setView(new L.LatLng(0,0), 0);
L.tileLayer.zoomify('https://pancreatic-ultrastructure.github.io/tuft-cell/tuftCell/', {
    width: 8192,
    height: 8192,
    tolerance: 0.5,
    attribution: 'Pancreatic ultrastructure'
}).addTo(map);
</script>
