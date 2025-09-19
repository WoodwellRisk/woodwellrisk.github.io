---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risks/fires/
---
# Wildfire

*When wildfires become out of control, they can destroy homes, impact habitats and cause large amounts of particulate matter (smoke), which can have significant impacts on human health.*


### Fire Weather Index
The Fire Weather Index (FWI) System (<a href='https://www.cabidigitallibrary.org/doi/full/10.5555/19910646918' target='_blank'>Wagner, 1987</a>; <a href='https://essd.copernicus.org/articles/15/2153/2023/' target='_blank'> Quilcaille et al., 2023 </a>) quantifies an area's wildfire potential using information about fuel availability, drought, and fire behavior. FWI has been used globally to assess wildfire risk at multiple scales and is based on meteorological variables only. We calculate daily FWI values using <a href='https://remo-rcm.de' target='_blank'>REMO2015</a>, a CMIP5-era monthly, high-resolution (0.2° or ~22km) regional climate model and an RCP8.5 emission scenario. The resulting FWI variable was then bias-adjusted (to ensure climate simulations match historical observations) using ISIMIP methodology (see **[Climate Data](/tools/climate-data/)**).

### Fire Danger Days <a href="https://woodwellrisk.github.io/viewer?layer=wdd" target="_blank"><img src="/assets/images/display-icon.svg" alt="display icon" style="width: 33px;"/></a>
Fire Danger Days are defined as those which exceed the historical (1970-2000) daily 95th percentile Fire Weather Index (i.e. the top 5% of all days between 1970 and 2000). With this metric, we calculate the historical 95th percentile FWI value and estimate how often that value is exceeded in the future.

###  Wildfire Smoke Deaths <a href="https://github.com/WoodwellRisk/smoke-mortality" target="_blank"><img src="/assets/images/github-icon.png" alt="GitHub icon" style="width:33px;"/></a>
Smoke exposure is a major health hazard, causing sickness and sometimes death from the respiratory and cardiovascular effects of increased PM2.5 inhalation. This means that an expected future increase in wildfires has important implications for human health, both for communities directly impacted by wildfires and those affected by smoke that is sometimes transported long distances. To estimate the change in smoke-related deaths from wildfires into the future, we make use of the future smoke emissions data and methodology from <a href='https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018GH000144' target='_blank'>Ford et al. (2018)</a>, with the constant for the hazard ratio chosen following <a href='https://ehp.niehs.nih.gov/doi/10.1289/ehp.1104049' target='_blank'>Crouse et al. (2012)</a>, to compare mortality projections for 2050 and 2100 with modeled estimates from 2000.

### Wildfire smoke and labor productivity
In addition to having serious impacts on human health, wildfire smoke has a noticiable, negative effect on labor productivity. Using future wildfire smoke emissions data, we can create an estimate of of productivity loss that takes into account population projections, annual work hours, and the productivity loss rate from <a href='https://www.aeaweb.org/articles?id=10.1257/app.20170286' target='_blank'>He et al. (2019)</a>. This allows us to view productivity loss projections attributable to wildfires for 2050 compared to modeled estimates from 2000, both in the form of total hours and work-years lost, to identify the most at-risk populations and countries.