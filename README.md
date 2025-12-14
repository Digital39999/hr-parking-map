# Croatia Parking Map

This repository contains the static map tiles used for a Croatia parking map.

The tiles are generated from OpenStreetMap data and exported as raster PNG tiles (`{z}/{x}/{y}.png`) from an MBTiles source.
They are intended to be served via GitHub Pages and consumed by a Leaflet-based frontend.

## Usage

Tiles can be used in Leaflet like this:

```js
L.tileLayer("https://<username>.github.io/<repo>/tiles/{z}/{x}/{y}.png", {
  maxZoom: 14,
  attribution: "© OpenStreetMap contributors",
}).addTo(map);
```
