---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /risk_tropical-cyclone/
---

# Tropical Cyclones

*Tropical cyclones (also known as hurricanes and typhoons) as powerful marine storms which can pose a significant threat to coastal communities. Their strong winds and rainfall can lead to widespread damage and dangerous coastal floods, posing a real threat to life. As rare extreme events, it is a challenge to assess their association risks from historical data alone. Therefore, statistical simulations are often used to evaluate their locations, wind speeds, rainfall and flooding under different climate scenarios.*

*For our tropical cyclone risk analyses, we use STORM synthetically generated tropical cyclones. This dataset offers 10,000 years of statistically generated tracks and intensities for every ocean globally and projects out to 2050. For more information on these tracks, see the following publications:*

<a href='https://www.nature.com/articles/s41597-020-0381-2' target='_blank'>Bloemendaal et al., (2020)</a>

<a href='https://www.science.org/doi/10.1126/sciadv.abm8438' target='_blank'>Bloemendaal et al., (2022)</a> 

### Intensity Return Periods <a href="https://github.com/WoodwellRisk/CRisk" target="_blank">![GH Logo](/assets/images/github-mark.png)</a>
We can use simulated tropical cyclone tracks to determine how often storms of different intensities approach a location. Specifically, for our analysis we look at storms passing within 100km. The distance from each storm center and grid point on a high resolution grid is calculated. Where this distance is less than or equal to 100km, the category of the storm (Tropical storm - category 5) is recorded. Across all storms and years, the number of storms passing each grid point is counted for each category, then divided by 10,000 to obtain the mean number of storms passing annually.

We are able to use this analysis to derive return periods and the number of storms per year.


### Wind Speed Return Periods <a href="https://github.com/WoodwellRisk/CRisk" target="_blank">![GH Logo](/assets/images/github-mark.png)</a>
The Holland model <a href='https://journals.ametsoc.org/view/journals/mwre/108/8/1520-0493_1980_108_1212_aamotw_2_0_co_2.xml' target='_blank'>(Holland, 1980)</a>  offers a way to expand synthetic tracks into 2 dimensional wind and pressure fields at the surface. By applying this model to 3000 years of simulated tracks, we can estimate reliable windspeed return periods around the world. To do this, we use the <a href='https://climada-python.readthedocs.io/en/stable/' target='_blank'>CLIMADA</a> Python toolbox, which offers workflows that can automate this analysis.