TRAINING POINTS — Land Use and Land Cover Classification Samples
================================================================

Description
-----------
Point samples used to train a Random Forest machine learning
classification model, applied over an Earth observation data cube built
from 16-day Brazil Data Cube (BDC) composites (Ferreira et al., 2020;
see References), using the SITS package
("Satellite Image Time Series Analysis on Earth Observation Data
Cubes" — Simões et al., 2021; see References). Samples cover the study
area for the years 2018-2024. Class definitions and visual
interpretation criteria are described in the accompanying file
"Chave_de_Classificacao_TESE.pdf" (classification key).

Study area
----------
Municipalities: Cruzeiro do Sul, Rodrigues Alves, Porto Walter, Mâncio
Lima (Acre) and Guajará (Amazonas), Brazil.
Sentinel-2 tiles: 18MXS, 18MYS, 18MZS, 18MXT, 18MYT, 18MZT, 18LXR,
18LYR, 18LZR.

Folder structure
-----------------
TRAINING/
  Chave_de_Classificacao_TESE.pdf   -> classification key (class descriptions)
  2018/TRAINING_POINTS_2018.shp (+ .shx, .dbf, .prj)
  2019/TRAINING_POINTS_2019.shp (+ .shx, .dbf, .prj)
  2020/TRAINING_POINTS_2020.shp (+ .shx, .dbf, .prj)
  2021/TRAINING_POINTS_2021.shp (+ .shx, .dbf, .prj)
  2022/TRAINING_POINTS_2022.shp (+ .shx, .dbf, .prj)
  2023/TRAINING_POINTS_2023.shp (+ .shx, .dbf, .prj)
  2024/TRAINING_POINTS_2024.shp (+ .shx, .dbf, .prj)

Format: ESRI Shapefile (point / multipoint geometry)

Coordinate Reference System (CRS)
----------------------------------
SIRGAS 2000 geographic (EPSG:4674) — standardized for all years, same
CRS used in VALIDATION/.

Attribute fields
-----------------
  id        : sample identifier (numeric)
  class     : land use / land cover class code, assigned through visual
              interpretation by the author (see legend below)
  longitude : longitude of the point (decimal degrees) [not present in 2019]
  latitude  : latitude of the point (decimal degrees)  [not present in 2019]

Class legend
------------
  AGPE - Small-Scale Agriculture        (Agricultura de Pequena Escala)
  AGUA - Water                          (Água)
  AL   - Floodable Areas                (Áreas Alagáveis)
  DMC  - Deforestation by Clear-Cutting (Desmatamento por Corte Raso)
  DMF  - Deforestation by Fire          (Desmatamento por Fogo)
  PA   - Shrub/Tree Pasture             (Pastagem Arbustiva/Arbórea)
  PH   - Herbaceous Pasture             (Pastagem Herbácea)
  PSI  - Fish Farming Ponds             (Tanques de Piscicultura)
  SE   - Exposed Soil                   (Solo Exposto)
  URB  - Urban Area                     (Urbanizada)
  VSA  - Advanced Secondary Vegetation  (Vegetação Secundária Avançada)
  VSI  - Initial Secondary Vegetation   (Vegetação Secundária Inicial)

Full visual interpretation criteria (shape, tone, texture, border, context,
temporal behavior) for each class are described in
"Chave_de_Classificacao_TESE.pdf".

Citation
--------
This dataset is part of an ongoing Master's thesis at the National
Institute for Space Research (INPE), Brazil, and has not yet been
published in a journal or conference. Please cite it via its Zenodo DOI:

  DOI: 10.5281/zenodo.22759288

License: CC-BY 4.0 (Creative Commons Attribution 4.0 International)

Author
------
Marcus Vinicius Gonçalves da Silva (ORCID: https://orcid.org/0009-0001-9904-9001)
National Institute for Space Research (INPE), Brazil
mvinicius.gsilva2003@gmail.com

References
----------
FERREIRA, K. R.; QUEIROZ, G. R.; VINHAS, L.; MARUJO, R. F. B.; SIMOES,
R. E. O.; PICOLI, M. C. A.; CAMARA, G. et al. Earth observation data
cubes for Brazil: Requirements, methodology and products. Remote
Sensing, v. 12, n. 24, p. 4033, 2020.

SIMÕES, R.; CÂMARA, G.; QUEIROZ, G.; SOUZA, F.; ANDRADE, P. R.; SANTOS, L.;
CARVALHO, A.; FERREIRA, K. Satellite image time series analysis for big
Earth observation data. Remote Sensing, v. 13, n. 13, p. 2428, 2021.
