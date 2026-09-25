# Viewshed Lab

Single-file browser viewshed explorer using WebGPU and public terrain data.

## Features

- Real-time curved-Earth viewshed and sight-distance rose
- WebGPU horizon computation and longest visible ray
- AEQD projection for large-area distance/azimuth fidelity
- Mapterhorn terrain with progressive detail and record-line refinement
- OSM and satellite basemaps reprojected into the local AEQD view
- Presets for documented long-distance sight lines
- Local browser persistence for UI and compute settings

## Run locally

```bash
python -m http.server 8000
```

Open `http://localhost:8000/` in a WebGPU-capable browser.

## Privacy

The application has no analytics or tracking. Browser geolocation is optional and user-triggered; saved location and settings remain in localStorage. Place search uses OpenStreetMap Nominatim only when explicitly submitted.

## Data / attribution

Elevation and basemap attribution is shown in-app. See the source links in the application for Mapterhorn, OpenStreetMap, Esri, GDAL, GRASS and related prior art.
