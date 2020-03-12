# HACKphoria
![Hackphoria](./hackphoria.jpg)

## Ideation:
 - A system for taxi cab drivers (or `Lyft`, `Uber`, etc) that takes their `GPS` tracks plus the `pickup/dropoff` times and locations and recommends loops to drive in that will likely put them near people that need a ride for a given time of day.(An app for taxi drivers..they could know which location to concentrate or go in loops so that they attract maximum customers)

## Google Maps API:
- Embeded map in page 
  ```html
  <div id="map"></div>
    <script>
      var map;
      function initMap() {
        map = new google.maps.Map(document.getElementById('map'), {
          center: {lat: -34.397, lng: 150.644},
          zoom: 8
        });
      }
    </script>
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap"
    async defer></script>
  ```
 - Map click event
  ```js 
  google.maps.event.addListener(map, 'click', function( event ){
  alert( "Latitude: "+event.latLng.lat()+" "+", longitude: "+event.latLng.lng() ); }); 
  ```
  # hello world
