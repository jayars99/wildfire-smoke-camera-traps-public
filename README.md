# wildfire-smoke-camera-traps-public
Reproducible code and final datasets for model selection, as well as data cleaning code from "Camera traps link population-level activity patterns with wildfire smoke events for mammals in Eastern Washington State," manuscript in preparation. Covariate cleaning code depends on camera trap location data not provided in this repository, which can be obtained by contacting the Washington Department of Fish and Wildlife.

Authors: Jessalyn Ayars, Robert L. Emmet, Sarah B. Bassing, Olivia V. Sanderfoot, Sierra Raby, Alexandra Karambelas, Eric P. James, Ravan Ahmadov, and Beth Gardner

Contents:

  code:

  - covariate-cleaning.Rmd - data-wrangling for site and observational covariates. Not runnable due to withheld data
  - detection-cleaning.Rmd - data-wrangling for detection histories for each species (name passed in). Runs from data.1.
  - models-species.Rmd - model selection code for each species
  - models-species.html - model selection output for each species
  - figures.Rmd - code for figure development. Partially runnable
  - map.Rmd - code for map (another figure). Not runnable

  data-raw:

  - detections.csv - detection data for all species for July - October 2018, 2019, and 2020. Locations removed.

  data-tidy:

  - poisson-data-species.csv - dataset used for Poisson regression for each species
  - dh-species.csv - detection history matrix used for occupancy modeling for each species
  - covs-site.csv - site covariates for camera traps
  - covs-obs-temp-scaled.csv - matrix of scaled temperatures at each camera trap each day for occupancy modeling
  - covs-obs-smoke-scaled.csv - matrix of scaled fire-specific PM 2.5 values at each camera trap each day for occupancy modeling
  - covs-obs-day-scaled.csv - matrix of scaled day-in-study values at each camera trap each day for occupancy modeling
  - stationsTbl.csv - camera trap setup, retrieval, and problem dates (locations removed)

  results:

  - species-pois-predictions.csv - predicted detections per day for a range of PM 2.5 values for species which responded to PM 2.5
  - map.tif - figure showing study area
  - pm25.tif - figure showing PM 2.5 levels throughout our study interval each year
  - poisson-figure-bobcat-moose.tif - figure showing bobcat and moose responses to PM 2.5 levels
  - poisson-figure-muledeer.tif - figure showing mule deer responses to PM 2.5 levels
  - species-occ-det.txt - text file of model results for the detection portion of the occupancy model for each species
  - species-occ-occ.txt - text file of model results for the occupancy portion of the occupancy model for each species
  - species-pois.txt - text file of model results for the poisson model for each species



