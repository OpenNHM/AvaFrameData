# avaChaiseren

## Event [15012019_3]

### Changelog
- V0 - Initial data assembly (27-07-2026)

### General description
This dataset is based on Glaus et al. (2025).

avaChaiseren is one of a total of three artificially released cold mixed flowing-powder avalanches (Wildi, Rüchi, Chaiseren) in the Dischma valley, near Davos.

#### Information about all three Braemabuehl events
 
- Terrain features: channelized below the release zone and a wide, laterally unconstrained runout zone at the valley bottom.
- Substantial snowfall before a cold spell; nearby snow-cover monitoring stations measured snow depths up to 2.5 m; strong winter storm on 14th of January redistributed snow on the slope. 
- The avalanches eroded a deep, cold snowpack and snow entrainment increased the avalanche mass after release. Further information regarding entrainment can be found in Glaus et al., (2025).
- All three avalanches developed a powder snow cloud; helicopter observations for the event series indicated runout-zone cloud speeds around 30 m s<sup>-1</sup> and cloud heights around 40 m.
- Post-event drone surveys allowed delineation of the release zone, mapping of snow-depth distribution and validation of runout length and deposition pattern.

#### Specific information about the Chaiseren avalanche
- Spatial parameters
    - Release area top elevation: 2240 m a.s.l.
    - Runout zone: 1570 m a.s.l.
    - Northeastern slope aspect
    - Measured runout distance: 1160 m
- Snow parameters
    - Release thickness: 95 cm
    - Maximum erosion height: 115 cm

### Available data
Data CRS: EPSG:2056

- release area (avaChaiseren_release_area.gpkg)
    - release thickness: 95 cm
- forest area (avaWildi_forest_area.gpkg)
    - polygons are defined according to expert judgement based on the orthophoto.
- avalanche area (avaChaiseren_avalanche_area.gpkg)
    - outline of all dense parts of the avalanche based on the orthophoto
- powder area (avaChaiseren_powder_area.gpkg)
    - rough estimation of the outlines of the powder cloud, identified from the orthophoto. 

The Orthophoto, acquired four days after the event (Braemabuehl_Ortho_20190119_0.04cm.tif) can be found at:https://doi.org/10.5281/zenodo.15796703

A digital elevation model (DEM) can be found at: https://www.swisstopo.admin.ch/de/hoehenmodell-swissalti3d 
- Use the DEM for the region "Davos (GR)" in 2 x 2 m resolution.
- If two tiles are necessary, do not forget to merge them before modelling.

### Data sources
- General description: Glaus, J., Wikstrom Jones, K., Bartelt, P., Christen, M., Stoffel, L., Gaume, J., & Bühler, Y. (2025). Simulation of cold-powder snow avalanches considering daily snowpack and weather situations. Natural Hazards and Earth System Sciences, 25(7), 2399-2419. DOI: https://doi.org/10.5194/nhess-25-2399-2025
- Data source: Brämabühl_Avalanche_Jan2019_Dataset DOI: https://doi.org/10.5281/zenodo.15796703
