---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risks/drought-water/
---

# Drought & Water Scarcity 
*Sufficient water is critical for sustaining life, public health and agriculture. The availability of water is not guaranteed however, and will change in the future thanks to changing weather patterns, growing populations and expanding industries. Drought is a crucial climate event that shapes water scarcity, posing serious challenges to those in charge of water management. In some areas, rising temperature and falling precipitation will increase the severity and frequency of extreme droughts, making it vital that we can accurately project when and where this is going to occur.*

### Palmer Drought Severity Index
The Palmer Drought Severity Index (<a href='https://climatedataguide.ucar.edu/climate-data/palmer-drought-severity-index-pdsi' target='_blank'>PDSI</a>) is a well-established drought indicator that describes anomalies in environmental water balance using monthly precipitation and evapotranspiration. This metric measures the magnitude of said anomalies both for historical and a future time period on a monthly basis. It is a normalized index ranging from -10 to +10, with negative (positive) values indicating dryer-than-normal (wetter) conditions.  Severe, or worse, drought is characterized by a PDSI value ≤ -3, and extreme drought has PDSI ≤ -4. 

We use the self-calibrated PDSI (<a href='https://journals.ametsoc.org/view/journals/clim/17/12/1520-0442_2004_017_2335_aspdsi_2.0.co_2.xml?tab_body=fulltext-display' target='_blank'>sc-PDSI</a>) which accounts for spatial variation in precipitation by calibrating to the local, historical climate. This enables comparable results over climatically diverse regions. sc-PDSI was computed using <a href='https://remo-rcm.de/' target='_blank'>REMO2015</a>, a CMIP5-era monthly, high-resolution (0.2° or ~22km) regional climate model, an RCP8.5 emission scenario, and a calibration time period of 1971–2000.

### Water Scarcity Index
This index is a relative global percentile ranking system derived from ten hydrological indicators: historical and future water stress, historical water depletion, future water supply, future water demand, future seasonal variability, historical interannual and seasonal variability of water supply, historical drought risk, and environmental flow limit.

Historical indicators are derived from Aqueduct 3.0, future indicators from Aqueduct Future, and environmental flow limit from <a href='https://www.nature.com/articles/s41586-019-1594-4' target='_blank'> de Graaf et al. (2019)</a>. Each indicator is standardized by resampling to ∼10 × 10 km using nearest neighbor sampling and remapping to an interval of 0–10 of increasing adverse (more water scarce) risk. Each indicator is weighted according to the default scheme developed by Aqueduct based on corporate water experts. Different weighting schemes relevant to specific industries can be applied. The standardized scores of all indicators of a single pixel are summed to give the pixel's total standardized score. All of the total standardized scores are then ranked by percentile. In the index, the overall score of a pixel is percentile rank, relative to the water scarcity of all other pixels around the world, with higher values representing more water scarce regions.