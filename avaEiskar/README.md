# avaEiskar

## Event 20190115 

### Changelog 

#### V1 -> V2

Renamed attributes for releaseEvent*; drop attributes for depositionPSAOutline*

#### V0 -> V1

Converted shapefiles to GeoPackage, renamed files and layers:

| Old file (pattern) | New file |
|---|---|
| `Ablagerung_Ereignis_Jan2019.*` | `depositionEvent20190115.gpkg` |
| `AnbruchDrone.*` | `releaseEvent20190115.gpkg` |
| `Entrainment_Smoothed.*` | `entrainmentEvent20190115.gpkg` |
| `Resistanced_Smoothed.*` | `resistanceEvent20190115.gpkg` |
| `Outline_DFA_Ablagerung.*` | `depositionDFAOutlineEvent20190115.gpkg` |
| `Outline_PSA_Ablagerung.*` | `depositionPSAOutlineEvent20190115.gpkg` |
| `Outline_Max_Ablagerung.*` | `depositionMaxOutlineEvent20190115.gpkg` |

#### V0

Initial commit with original file names

---

### General description 
- Type of avalanche: dense flow with major powder cloud, dry snow
- Entrainment: Significant for avalanche formation
- Date: 15.01.2019 
- Be aware: the release file has two release areas ESK1 and ESK2. Relevant for the runout at the bottom is 
  only ESK1 (reasoning see report pdf in this repository; German only)
- Drone scan data from a flight on 18.01.2019 is available too, and will be published in future.  
- Release thickness and outline is based on this drone laser scan. 

### Available data

| File | Geometry | Description                                                                                                                                               |
|---|---|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| `depositionEvent20190115.gpkg` | LineString | Deposition outline of the event. Based on where effects <br/>could be seen either on the orthofoto or local observations                                  |
| `releaseEvent20190115.gpkg` | 3D Polygon | Release areas ESK1 and ESK2 (drone-derived); attributes see below                                                                                         |
| `entrainmentEvent20190115.gpkg` | Polygon | Entrainment areas (smoothed)                                                                                                                              |
| `resistanceEvent20190115.gpkg` | Polygon | Resistance areas (smoothed)                                                                                                                               |
| `depositionDFAOutlineEvent20190115.gpkg` | Polygon | Dense flow avalanche deposition outline; derived from laser scan data  <br/>                                                                              |
| `depositionPSAOutlineEvent20190115.gpkg` | Polygon | Powder snow avalanche deposition outline; derived from laser scan data; i.e. where <br/>considerable amounts of deposition can be extracted from the data |
| `depositionMaxOutlineEvent20190115.gpkg` | Polygon | Maximum deposition outline (DFA + PSA combined); derived from laser scan data                                                                             |

Note: the difference between `depositionEvent` and `depositionMaxOutlineEvent` is the derivation of it. The 
`depositionEvent` is based purely on (visual) observations (orthophoto and local), while `depositionMaxOutlineEvent` 
is based on laser scan data, i.e. where considerable deposition masses can be shown. 

### Attributes

#### `releaseEvent20190115.gpkg`

| Attribute | Type | Description |
|---|---|---|
| `elevation_bottom` | Integer64 | Elevation of the lower release area boundary (m) |
| `elevation_top` | Integer64 | Elevation of the upper release area boundary (m) |
| `elevation_drop` | Integer64 | Vertical drop from top to bottom (m) |
| `slope_deg` | Real | Average slope angle (degrees) |
| `area_2d` | Integer64 | Planar release area (m²) |
| `area_3d` | Integer64 | Surface release area in 3D (m²) |
| `date` | String(20) | Date of the release area mapping |
| `source` | String(50) | Data source and provenance |
| `volume_3d` | Real | Release volume (m³) |
| `name` | String(80) | Release area identifier (e.g. ESK1, ESK2) |
| `thickness` | Real | Release thickness in (m) |

### Data source

WLV (Austrian Avalanche and Torrent Service)

