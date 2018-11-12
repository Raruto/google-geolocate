# google-geolocate.js
A Google Maps plugin that adds a geolocation control.

_For a working example see [demo](https://raruto.github.io/examples/google-geolocate/google-geolocate.html)
---

## How to use

1. **include CSS & JavaScript**
    ```html
    <head>
    ...
    <style>html, body, #map { width: 100%; height: 100%; margin: 0; padding: 0; }</style>
    <script src="https://maps.google.com/maps/api/js?key="></script>
    <script src="https://raruto.github.io/cdn/google-geolocate/0.0.1/google-geolocate.js"></script>
    ...
    </head>
    ```
2. **choose the div container used for the slippy map**
    ```html
    <body>
    ...
    <div id="map"></div>
    ...
    </body>
    ```
3. **create your first simple “google-geolocate” slippy map**
    ```html
    <script>
      var mapOpts = {
        center: new google.maps.LatLng(45, 9.5),
        zoom: 5,
        MapTypeId: google.maps.MapTypeId.ROADMAP
      };

      var map = new google.maps.Map(document.getElementById('map'), mapOpts);
      var geolocationControl = new GeolocationControl(map, 13);
    </script>
    ```

---

**Compatibile with:** gmaps@3.34

---

**Contributors:** [Raruto](https://github.com/Raruto/google-geolocate)
