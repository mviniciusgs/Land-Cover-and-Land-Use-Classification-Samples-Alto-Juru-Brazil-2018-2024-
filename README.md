This dataset provides the training and validation point samples, along with
accuracy assessment figures, used in a land use and land cover (LULC)
classification of the Alto Juruá region (Acre and Amazonas states, Brazil),
covering the years 2018-2024.

The classification was produced with a Random Forest machine learning model
applied over an Earth observation data cube built from 16-day Brazil Data
Cube (BDC) composites, using the SITS package (Simões et al., 2021).
Accuracy assessment followed the design-based good-practice recommendations
of Olofsson et al. (2014).

The dataset is organized into three parts:
- TRAINING: point samples (ESRI Shapefile) used to train the classification
  model for each year.
- VALIDATION: independent reference point samples (ESRI Shapefile) used for
  accuracy assessment.
- VALIDATION_IMAGES: accuracy comparison charts and confusion matrices for
  each year, including three alternative classification experiments run for
  2024 (data cube composition, segmentation, and Self-Organizing Map).

All points use the SIRGAS 2000 geographic CRS (EPSG:4674). A classification
key (PDF) describing each of the 12 land use/land cover classes (visual
interpretation criteria: shape, tone, texture, border, context and temporal
behavior) is included in every folder.

This dataset is part of an ongoing Master's thesis at the National Institute
for Space Research (INPE), Brazil, and has not yet been published in a
journal or conference.
