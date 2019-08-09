```
function drawMap(data) {
+  var options = {
+  pointToLayer: function (feature, latlng) {
+      return L.circleMarker(latlng, geojsonMarkerOptions)
+  }
    L.geoJson(data, options).addTo(map);
}
```
