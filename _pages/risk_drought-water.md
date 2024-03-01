---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risk_drought-water/
---


### Drought PDSI
The Palmer Drought Severity Index ([PDSI](https://climatedataguide.ucar.edu/climate-data/palmer-drought-severity-index-pdsi)) is a well-established drought indicator that describes environmental water balance using monthly precipitation and evapotranspiration. This metric measures the annual average months with drought at, or below, a specified level based on monthly PDSI index, and the projected change in months for a future time period. It is a normalized index ranging from -10 to +10, with negative (positive) values indicating dry (wet) conditions.  Severe, or worse, drought is characterized by a PDSI value ≤ -3, and extreme drought has PDSI ≤ -4. The self-calibrated PDSI ([sc-PDSI](https://journals.ametsoc.org/view/journals/clim/17/12/1520-0442_2004_017_2335_aspdsi_2.0.co_2.xml?tab_body=fulltext-display)) was used here, which accounts for spatial variation in precipitation by calibrating to the local, historical climate. This enables comparable results over climatically diverse regions. sc-PDSI was computed using [REMO2015](https://remo-rcm.de/), a CMIP5-era monthly, high-resolution (0.2° or ~22km) regional climate model, an RCP8.5 emission scenario, and a calibration time period of 1971–2000.


### Water Scarcity Index
This index is a relative global percentile ranking system based on ten hydrological indicators: historical and future water stress, historical water depletion, future water supply, future water demand, future seasonal variability, historical interannual and seasonal variability of water supply, historical drought risk, and environmental flow limit.

The historical indicators are derived from Aqueduct 3.0, future indicators from Aqueduct Future, and environmental flow limit from de Graaf et al., 2019. Each indicator is standardized by resampling to ∼10 × 10 km using nearest neighbor sampling and remapping to an interval of 0–10 of increasing adverse (more water scarce) risk. Each indicator is weighted according to the default scheme developed by Aqueduct based on corporate water experts. Different weighting schemes relevant to specific industries can be applied. The standardized scores of all indicators of a single pixel are summed to give the pixel's total standardized score. All of the total standardized scores are then ranked by percentile. In the index, the overall score of a pixel is percentile rank, relative to the water scarcity of all other pixels around the world, with higher values representing more water scarce regions. 

