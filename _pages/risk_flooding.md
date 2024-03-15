---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risk_flooding/
---

### Flood Modelling
Coastal and inland flood risk is simulated using the LISFLOOD-FP flood model <a href="https://gmd.copernicus.org/articles/16/2391/2023/" target="_blank">(Sharifian et al., 2022)</a>. LISFLOOD-FP takes into account streamflow, rainfall, storm surge, land cover, and soil infiltration to estimate maximum flood depth. Dynamics between surface flow and stormwater systems can be modeled using a coupling framework between LISFLOOD-FP and Stormwater Management Model <a href="https://www.epa.gov/water-research/storm-water-management-model-swmm" target="_blank">(SWMM)</a> that was developed in-house. We are able to simulate flooding at high spatial resolutions ranging from less than 5 meters to 30 meters.

### Sea Level Rise Inundation Extent
Sea level rise inundation is mapped globally at a 30-meter resolution using our internally developed global DEM (see <a href="/tools_diluvium/">DiluviumDEM</a>) or local DEMs where available. Local sea level rise projections are from the <a href="https://sealevel.nasa.gov/data_tools/17" target="_blank">NASA IPCC AR6</a> dataset <a href="https://doi.org/10.1017/9781009157896.011" target="_blank">(Fox-Kemper et al., 2021)</a>. These projections take into account ocean thermal expansion, glacial and ice cap melting, and subsidence. The coastal water levels of the annual flood (1-year return period) are added to the sea level rise projections to represent the highest yearly water level around the globe <a href="https://www.frontiersin.org/articles/10.3389/fmars.2020.00263/full" target="_blank">(Muis et al., 2020)</a>. Finally, a bathtub approach in conjunction with a connected components analysis is used to estimate future annual inundation from sea level rise.