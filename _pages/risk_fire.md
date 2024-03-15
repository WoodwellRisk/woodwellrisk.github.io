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
The Fire Weather Index (<a href='https://essd.copernicus.org/articles/15/2153/2023/' target='_blank'>FWI</a>) System quantifies ecosystem vulnerability to wildfire and wildfire potential. It addresses fuel availability, drought, and fire behavior using seven indices: Buildup Index, Daily Severity Rating, Drought Code, Duff Moisture Code, Fine Fuel Moisture Code, Fire Weather Index, and Initial Spread Index. FWI has been used globally to assess wildfire risk at multiple scales and is based on meteorological variables only. We calculate daily FWI values using <a href='https://remo-rcm.de' target='_blank'>REMO2015</a>, a CMIP5-era monthly, high-resolution (0.2° or ~22km) regional climate model and an RCP8.5 emission scenario. The resulting FWI variable was then bias-adjusted (to ensure climate simulations match historical observations) using ISIMIP methodology (see **[Climate Data](/tool_data/)**).

### Fire Danger Days
Fire Danger Days are defined as those which exceed the daily 95th percentile Fire Weather Index (i.e. the top 5% of FWI values or about 18 days per year). With this metric, we calculate the historical 95th percentile FWI value and estimate how often that value is exceeded in the future.

