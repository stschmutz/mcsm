title: Clubraum
date: 18.02.2015
---
## Clubraum

Die Clubr&auml;me des MSCM befinden sich im Sirius Business Park in der Rupert-Mayer-Str. 44.  Du kann mit der U3 bis zur Station &quot;Obersendling&quot; oder mit der S3, bis zur Station &quot;Siemenswerke&quot; fahren. Von dort sind es 5-10 Minuten zum Haupteingang.

<div id="map-canvas"></div>
<script src="https://maps.googleapis.com/maps/api/js?v=3.exp"></script>

<img src="/images/sirius_main-fs8.png" />

F&uuml;r den ersten Besuch bietet es sich an beim Pf&ouml;rtner am Haupteingang das Gel&auml;nde zu betreten und sich den Weg erkl&auml;ren zu lassen.

<img src="/images/sirius_entrance-fs8.png" />

Die Seiteneing&auml;nge k&ouml;nnen nur als Ausg&auml;nge benutzt werden.

<img src="/images/mcsm_road-fs8.png" />

## Adresse

Modellbauclub der Siemens Mitarbeiter M&uuml;nchen e.V.
Sirius Business Park
Ruppert Mayer-Str.44
81379 M&uuml;nchen
Geb&auml;ude 6415, Raum 169

<script>

function initialize() {
  var mapOptions = {
    zoom: 17,
    center: new google.maps.LatLng(48.095, 11.533),
    mapTypeId: google.maps.MapTypeId.TERRAIN,
    zoomControl: true,
    streetViewControl: false,
    zoomControlOptions: {
      style: google.maps.ZoomControlStyle.LARGE
    }
  };

  var map = new google.maps.Map(document.getElementById('map-canvas'),
      mapOptions);

  var myLatlng = new google.maps.LatLng(48.0959845,11.5353281)

  var marker = new google.maps.Marker({
      position: myLatlng,
      map: map,
      title: 'MCSM'
  });

}

google.maps.event.addDomListener(window, 'load', initialize);

</script>
