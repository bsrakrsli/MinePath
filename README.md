<img width="1190" height="678" alt="Ekran Resmi 2026-07-16 01 51 58" src="https://github.com/user-attachments/assets/4eb9ae34-3a9c-4b6d-bb50-9e0dc29c4e29" />
# MinePath – Interactive Haul Road Route Editor

MinePath is a lightweight web-based GIS application developed as a demonstration of manual haul road digitization and route comparison for open-pit mining operations.

The application allows users to draw existing and optimized haul truck routes directly on high-resolution satellite imagery and dynamically estimates operational metrics such as distance, average slope, fuel consumption, travel time, and operational cost.
app screen
<img width="1190" height="678" alt="Ekran Resmi 2026-07-16 01 51 58" src="https://github.com/user-attachments/assets/881757c3-ce35-4bbc-aae4-503775b2e158" />

---

## Features

- Interactive haul road digitization
- High-resolution satellite imagery (Esri World Imagery)
- Multiple open-pit mine locations
- Current vs Optimized route comparison
- Dynamic calculation of:

  - Route distance
  - Average slope (pseudo DEM model)
  - Fuel consumption
  - Travel time
  - Operational cost

- Multiple haul truck models

  - CAT 785C
  - CAT 793F
  - Komatsu 930E
  - BELAZ 75710

- Coordinate export in JSON format

---

## Demo

Current Route (red dashed)

Optimized Route (green)

Interactive point editing

Undo last point

Clear routes

Coordinate export

---

## Technologies

- HTML5
- CSS3
- JavaScript
- Leaflet.js
- Esri World Imagery

---

## Route Analysis

The application estimates route performance using:

Distance

Average Slope

Fuel Consumption

Travel Time

Operational Cost

Since no real Digital Elevation Model (DEM) is used, elevation values are generated using a pseudo-elevation function for demonstration purposes.

In real mine planning software, slope calculations would typically be derived from:

- DEM
- LiDAR
- Drone Photogrammetry
- Mine Survey Data

---

## Mine Locations

The application currently includes three example open-pit mines:

- Bingham Canyon Mine (USA)
- Chuquicamata Mine (Chile)
- Morenci Mine (USA)

---

## Coordinate Export

Routes can be exported as JSON.

Example:

```json
{
  "currentRoute": [
    [40.5233, -112.1500],
    [40.5241, -112.1512]
  ],
  "optimizedRoute": [
    [40.5235, -112.1490],
    [40.5245, -112.1505]
  ]
}
```

---

## Future Improvements

- Real DEM integration
- Automatic shortest path calculation
- A* pathfinding algorithm
- Dijkstra routing
- Truck speed modelling
- Elevation profile
- Cost optimization
- GeoJSON import/export
- Shapefile support
- Slope heatmap
- Real mine road network analysis

---

## Disclaimer

This application is intended as a proof-of-concept and educational demonstration.

The slope calculations are generated using a pseudo-elevation model and do not represent actual terrain elevations.

---

## License

MIT License
