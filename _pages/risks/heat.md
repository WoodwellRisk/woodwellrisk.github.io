---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risks/heat/
---
# Heat

*Extreme temperatures and humidity levels can pose significant risks to public health. Extreme conditions can lead to heat-related illnesses such as heat exhaustion and heatstroke, particularly in vulnerable populations like the elderly and young children. With climate change, these risks are expected to increase for many regions around the world. Our heat analyses allows us to understand how and where these risks are likely to change in the future*.

### Lethal Heat <a href="https://github.com/WoodwellRisk/lethal_heat" target="_blank"><img src="/assets/images/github-icon.png" alt="GitHub icon" style="width: 33px;"/></a> <a href="https://woodwellrisk.github.io/viewer?layer=lethal_heat" target="_blank"><img src="/assets/images/display-icon.svg" alt="display icon" style="width: 33px;"/></a>
In very hot or very humid conditions, heat can become lethal to people exposed for extended periods of time. This metric uses experimental evidence from <a href='https://pubmed.ncbi.nlm.nih.gov/34913738' target='_blank'>Vecellio et al. (2022)</a> to estimate when and where 'lethal' temperature and humidity occurs from an ensemble of global climate datasets.  

For more information, see our publication <a href='https://www.science.org/doi/10.1126/sciadv.adg9297' target='_blank'>Powis et al. (2023)</a>.

### Extreme Heat
Many communities will have some level of adaptation to their historical temperature conditions. Our Extreme Heat metric calculates the temperature at which only 5% of days exceed during a baseline period and estimates how often that will occur under future climates. This is useful to examine how historical adaptation measures will be challenged. To calculate this, we use daily temperature data from 17 CMIP6 ensemble members, which have been bias adjusted and downscaled (see **[Climate Data](/tools/climate-data/)**). 

### Heat Danger Days
Heat Index (see <a href='https://www.weather.gov/ama/heatindex' target='_blank'>here</a>) combined temperature and relative humidity to estimate the temperature perceived by humans. The National Weather Service defines 39.4C (103F) as a 'dangerous' threshold. Above this threshold, exposed people may experience heat cramps, exhaustion and possibly heast stroke. To calculate this, we use daily temperature data from 17 CMIP6 ensemble members, which have been bias adjusted and downscaled (see **[Climate Data](/tools/climate-data/)**)

### Lost Productivity <a href="https://github.com/WoodwellRisk/Lost_Productivity" target="_blank"><img src="/assets/images/github-icon.png" alt="GitHub icon" style="width: 33px;"/></a>

When workers are exposed to high temperatures and high humidity, their health can be significantly impacted, which in turn can have consequences for productivity. For this metric, we can analyse ensembles of climate data to estimate percentage losses in producivity of medium and heavy outdoor workers. 

This metric is based on work by <a href='https://www.nature.com/articles/s41467-021-27328-y#data-availability' target='_blank'>Parsons et al. (2021)</a> , which you can view for more methodology information.