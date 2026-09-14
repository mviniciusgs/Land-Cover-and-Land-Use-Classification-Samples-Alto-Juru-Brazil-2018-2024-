VALIDATION POINTS — Accuracy Assessment Samples
==================================================

Description
-----------
Independent reference point samples used for accuracy assessment of the
land use/land cover classification, for the years 2018-2024, following
the design-based good-practice recommendations of Olofsson et al. (2014;
see References). Class definitions and visual interpretation criteria
are described in the accompanying file "Chave_de_Classificacao_TESE.pdf"
(classification key).

Study area
----------
Municipalities: Cruzeiro do Sul, Rodrigues Alves, Porto Walter, Mâncio
Lima (Acre) and Guajará (Amazonas), Brazil.
Sentinel-2 tiles: 18MXS, 18MYS, 18MZS, 18MXT, 18MYT, 18MZT, 18LXR,
18LYR, 18LZR.

Folder structure
-----------------
VALIDATION/
  Chave_de_Classificacao_TESE.pdf   -> classification key (class descriptions)
  2018/VALIDATION_POINTS_2018.shp (+ .shx, .dbf, .prj)
  2019/VALIDATION_POINTS_2019.shp (+ .shx, .dbf, .prj)
  2020/VALIDATION_POINTS_2020.shp (+ .shx, .dbf, .prj)
  2021/VALIDATION_POINTS_2021.shp (+ .shx, .dbf, .prj)
  2022/VALIDATION_POINTS_2022.shp (+ .shx, .dbf, .prj)
  2023/VALIDATION_POINTS_2023.shp (+ .shx, .dbf, .prj)
  2024/VALIDATION_POINTS_2024.shp (+ .shx, .dbf, .prj)

Format: ESRI Shapefile (point geometry)

Coordinate Reference System (CRS)
----------------------------------
SIRGAS 2000 geographic (EPSG:4674) — standardized for all years, same
CRS used in TRAINING/.

Attribute fields
-----------------
  fid     : sequential point identifier (1, 2, 3, ...)
  REVISOR : reference land use / land cover class code, assigned through
            visual interpretation by the author (same class legend as
            TRAINING/)

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
OLOFSSON, P.; FOODY, G. M.; HEROLD, M.; STEHMAN, S. V.; WOODCOCK, C. E.;
WULDER, M. A. Good practices for estimating area and assessing accuracy
of land change. Remote Sensing of Environment, v. 148, p. 42–57, 2014.
