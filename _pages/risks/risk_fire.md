---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risk_fire/
---
# Wildfire

*When wildfires become out of control, they can destroy homes, impact habitats and cause large amounts of particulate matter (smoke), which can have significant impacts on human health.*


### Fire Weather Index
The Fire Weather Index (FWI) System (<a href='https://www.cabidigitallibrary.org/doi/full/10.5555/19910646918' target='_blank'>Wagner, 1987</a>; <a href='https://essd.copernicus.org/articles/15/2153/2023/' target='_blank'>Quilcaille et al., 2023</a>) quantifies an area's wildfire potential using information about fuel availability, drought, and fire behavior. FWI has been used globally to assess wildfire risk at multiple scales and is based on meteorological variables only. We calculate daily FWI values using <a href='https://remo-rcm.de' target='_blank'>REMO2015</a>, a CMIP5-era monthly, high-resolution (0.2° or ~22km) regional climate model and an RCP8.5 emission scenario. The resulting FWI variable was then bias-adjusted (to ensure climate simulations match historical observations) using ISIMIP methodology (see **[Climate Data](/tools_climate-data/)**).

### Fire Danger Days
Fire Danger Days are defined as those which exceed the historical (1970-2000) daily 95th percentile Fire Weather Index (i.e. the top 5% of all days between 1970 and 2000). With this metric, we calculate the historical 95th percentile FWI value and estimate how often that value is exceeded in the future.