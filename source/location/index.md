title: The Location
date: 2014-09-05 19:24:08
---

## How to find us

The MSCM is located at Sirius Business Park (form. Siemenswerke) at Rupert-Mayer-Str. 44.  You can get there either with U3, station "Obersendling", or S3, station "Siemenswerke".

<div id="map-canvas"></div>
<script src="https://maps.googleapis.com/maps/api/js?v=3.exp"></script>

## Finding Geb. 

There are side entrances but if it is better to access the area at the main entrance.

<img src="/images/mcsm_road.png" />


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

  var myLatlng = new google.maps.LatLng(48.0950069,11.5335578)

  var marker = new google.maps.Marker({
      position: myLatlng,
      map: map,
      title: 'MCSM'
  });

}

google.maps.event.addDomListener(window, 'load', initialize);

</script>
