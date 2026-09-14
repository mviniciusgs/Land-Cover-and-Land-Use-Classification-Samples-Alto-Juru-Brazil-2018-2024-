VALIDATION IMAGES — Accuracy Assessment Charts and Confusion Matrices
========================================================================

Description
-----------
Figures generated from the accuracy assessment of the classification:
global/combined accuracy comparisons, confusion matrices, and area
comparisons, for each year (2018-2024) and, for 2024, also for three
alternative classification experiments. The accuracy assessment follows
the design-based good-practice recommendations of Olofsson et al. (2014;
see References). Class codes appearing in the charts follow the same
legend as TRAINING/ and VALIDATION/, described in
"Chave_de_Classificacao_TESE.pdf".

Study area
----------
Municipalities: Cruzeiro do Sul, Rodrigues Alves, Porto Walter, Mâncio
Lima (Acre) and Guajará (Amazonas), Brazil.
Sentinel-2 tiles: 18MXS, 18MYS, 18MZS, 18MXT, 18MYT, 18MZT, 18LXR,
18LYR, 18LZR.

Folder structure
-----------------
VALIDATION_IMAGES/
  Chave_de_Classificacao_TESE.pdf   -> classification key (class descriptions)

  2018/ ... 2023/
    Global_Accuracy_Comparison.png
    Combined_Accuracy_Comparison_AGPE.png
    Combined_Accuracy_Comparison_AllLabels.png
    Confusion_Matrix_Individual_<year>.png

  2024/
    Global_Accuracy_Comparison.png
    Combined_Accuracy_Comparison_AGPE.png
    Combined_Accuracy_Comparison_AllLabels.png
    Confusion_Matrix_Individual_2024.png
    (validation images of the FINAL 2024 classification)

    Experiments/
      Cube_Composition/   -> validation images of the "data cube composition" experiment
      Segmentation/        -> validation images of the "segmentation" experiment
        (methods compared: Felzenszwalb-Huttenlocher, Region Growing, SNIC)
      SOM/                  -> validation images of the "Self-Organizing Map" experiment

Image types
-----------
  Global_Accuracy_Comparison*         : overall/global accuracy comparison chart
  Combined_Accuracy_Comparison_AGPE*  : combined accuracy chart, restricted to
                                         the Small-Scale Agriculture (AGPE) class
  Combined_Accuracy_Comparison_AllLabels* : combined accuracy chart, all classes
  Confusion_Matrix_Individual*        : confusion matrix for that year/method
  Area_Comparison_All / _Filtered     : comparison of mapped areas (raw / filtered)
  Error_Composition_AGPE_Bars         : error composition bar chart (AGPE class)
  Fragment_Size_Comparison_AGPE_PA_PH : fragment size comparison, AGPE/PA/PH classes

Experiment configuration codes (2024/Experiments/Cube_Composition)
--------------------------------------------------------------------
These codes identify which data cube features were used as input in each
classification experiment:
  DB_B      : Bands only
  DB_B_S    : Bands + Segments
  DB_B_IS   : Bands + Spectral Indices
  DB_B_FULL : Bands + Spectral Indices + Segments (full feature set)

Segmentation algorithms (2024/Experiments/Segmentation)
-----------------------------------------------------------
  FELZENSZWALB    : Felzenszwalb-Huttenlocher graph-based segmentation
                     algorithm (Felzenszwalb & Huttenlocher, 2004; see
                     References)
  REGION_GROWING  : Region Growing segmentation algorithm, GRASS GIS
                     i.segment module (Momsen & Metz, 2012; see References)
  SNIC            : Simple Non-Iterative Clustering segmentation
                     algorithm (Achanta & Süsstrunk, 2017; see References)

SOM configuration codes (2024/Experiments/SOM)
---------------------------------------------------
  SOM_2-4-12-13-23-91 : Self-Organizing Map neuron subset {2,4,12,13,23,91}
  SOM_N_91             : Self-Organizing Map with 91 neurons

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

ACHANTA, R.; SÜSSTRUNK, S. Superpixels and polygons using simple
non-iterative clustering. In: IEEE CONFERENCE ON COMPUTER VISION AND
PATTERN RECOGNITION (CVPR), 2017, Honolulu. Proceedings [...], p.
4651–4660, 2017.

FELZENSZWALB, P. F.; HUTTENLOCHER, D. P. Efficient graph-based image
segmentation. International Journal of Computer Vision, v. 59, n. 2,
p. 167–181, 2004.

MOMSEN, E.; METZ, M. i.segment: Identifies segments (objects) from
imagery data. GRASS Development Team, 2012. Manual eletrônico.
Disponível em: https://grass.osgeo.org/grass-stable/manuals/i.segment.html.
Acesso em: 29 jun. 2026.
