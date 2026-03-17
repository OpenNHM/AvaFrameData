# avaFilisur2

## Event [23022012_2]

### Changelog 
- V0 - Initial data assembly (05-12-2025)

### General description
Based on Feistl et al. (2014)

- Location: Filisur, Switzerland
- Date: 23.02.2012
- Elevation: Release area at 1360 m a.s.l, runout at 1058 m a.s.l
- Slope Angle, release to runout: 50-20°
- Release Volume: 1390 m³ (derived from mapped release areas combined with an assumend/estimated fracture depth - Feistl et al. 2014)
- Terrain features (upper part/track/runout): channeled/unchanneled/unchanneled
- Forest strucure (upperpart/track/runout): no forest/open/dense
    - approx. 500 stems/ha, tree groups with low-hanging branches
    - mixed tree age
- Avalanche Type: wet snow avalanche
- Temperature (dry/moist/wet): wet 
- Key Field Observations: 
    - Most avalanche mass was stopped at the forest edges, resulting in large wedge-shaped deposits along the sides of the main flow channel.
    - The main avalanche channel was largely open and not forested.

### Available data
All event layers were originally in LV03 (EPSG:21781). Since SwissTopo DEMs are in LV95 (EPSG:2056), all layers were reprojected to EPSG:2056 to avoid misalignment.

- release area (avaFilisur2_release_area.gpkg)
    - no documented thickness
    - Feistl et al. 2014 used a standardized thickness of 1m for their modelling process
- forest area (avaFilisur2_forest_area.gpkg)
    - Based on Feistl et al. (2014), forest classes are defined by canopy density: stands with >50% canopy cover are classified as "dense", those with <50% as "open", based on 25cm-resolution orthophotos.
- deposition area (avaFilisur2_deposition_area.gpkg)
    - no documented thickness

A digital elevation model (DEM) can be found at: https://www.swisstopo.admin.ch/de/hoehenmodell-swissalti3d 
- Use the DEM for the region "Bergün Filisur (GR) in 2x2m resolution.
- If two tiles are necessary, don´t forget to merge them before modelling.  


### Data source 
- General Description: Feistl, T., Bebi, P., Teich, M., Bühler, Y., Christen, M., Thuro, K., & Bartelt, P. (2014). Observations and modeling of the braking effect of forests on small and medium avalanches. Journal of Glaciology, 60(219), 124-138.
- Data Sources: provided by SLF Davos