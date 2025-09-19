---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /tools/climate-data/
---

# Our Climate Data

*We use climate data from multiple sources in our analyses and much of that data requires preprocessing steps.*

**Bias adjustment:** *All climate models contain biases, which can vary across the globe. To ensure we can offer the best climate risk assessments possible, we attempt to remove them before using the climate data ensemble in our analyses.*

**Downscaling:** *Global Climate Model ( GCM ) outputs, such as those from CMIP6, typically provide climate data at spatial resolutions of 1° to 2°, which is of limited utility for local and regional assessments. Downscaling methods use statistical or dynamic approaches to enhance the resolution of climate model data.*

*Our primary source of climate model data is the Coupled Model Intercomparison Project 6 ( CMIP6 ). These data are comprised of output from a large ensemble of model runs performed at a variety of institutions across the world.* 

### ISIMIP Bias Adjustment & Downscaling
For bias adjustment and statistical downscaling (BASD) of the majority of our climate variables, we use the <a href="https://zenodo.org/records/7151476" target="_blank">ISIMIP3BASD v2.5</a> framework. See <a href="https://gmd.copernicus.org/articles/12/3055/2019/" target="_blank">here</a> and <a href="https://www.isimip.org/documents/413/ISIMIP3b_bias_adjustment_fact_sheet_Gnsz7CO.pdf" target="_blank">here</a> for more information on this procedure.

### CHELSA 1km Downscaling <a href="https://github.com/WoodwellRisk/CHELSA_downscaling" target="_blank"><img src="/assets/images/github-icon.png" alt="GitHub icon" style="width:33px;"/></a>

We use the CHELSA method to obtain very high resolution downscaled monthly climatologies of mean, minimum and maximum air temperature, precipitation and nineteen bioclimatic variables. The <a href="https://pypi.org/project/chelsa-cmip6/" target="_blank">CHELSA</a> method statistically downscales monthly climatologies of these variables to 1 km spatial resolution globally. The method was developed at the Swiss Federal Institute for Forest, Snow and Landscape Research ( WSL ) and is based on the climatologies at high resolution for the earth’s land surface areas (CHELSA) <a href="https://chelsa-climate.org/" target='_blank'>dataset</a>. We have adapted CHELSA so that downscaling can be performed for user specified locations, time periods or warming levels, CMIP6 models, and scenarios.

For the full description on how we use the CHELSA method, see our <a href='/assets/pdfs/Downscaling CMIP6 data with CHELSA.pdf' target='_blank'>report</a>.

