# avaEiskar

## Event 20190115 

### Changelog 

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
  only ESK1 (reasoning see report pdff in this repository; German only)
- Drone scan data from a flight on 18.01.2019 is available too, and will be published in future.  

### Available data

| File | Geometry | Description |
|---|---|---|
| `depositionEvent20190115.gpkg` | LineString | Deposition outline of the event |
| `releaseEvent20190115.gpkg` | 3D Polygon | Release areas ESK1 and ESK2 (drone-derived) |
| `entrainmentEvent20190115.gpkg` | Polygon | Entrainment areas (smoothed) |
| `resistanceEvent20190115.gpkg` | Polygon | Resistance areas (smoothed) |
| `depositionDFAOutlineEvent20190115.gpkg` | Polygon | Dense flow avalanche deposition outline |
| `depositionPSAOutlineEvent20190115.gpkg` | Polygon | Powder snow avalanche deposition outline |
| `depositionMaxOutlineEvent20190115.gpkg` | Polygon | Maximum deposition outline (DFA + PSA combined) |


### Data source

WLV (Austrian Avalanche and Torrent Service)



