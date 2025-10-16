---
template: main.html

hide:
  - toc
  - path
---

# Tropical Cyclones <a href="https://github.com/WoodwellRisk/CRisk" target="_blank">:simple-github:{ .md }</a> <a href="https://woodwellrisk.github.io/viewer?category=coastal-risk&layer=tc_rp" target="_blank">:material-monitor:{ .md }</a>

Tropical cyclones (also known as hurricanes and typhoons) are powerful marine storms which can pose a significant threat to coastal communities. Their strong winds and rainfall can lead to widespread damage and dangerous coastal flooding, posing a real threat to life and property. Since high quality satellite records of these storms go back only a few decades, it is a challenge to assess their associated risks from historical data alone. Therefore, statistical simulations offer a valuable tool to evaluate storm locations, wind speeds, rainfall and flooding under different climate scenarios.

We analyse tropical cyclone risk by generating thousands of years of simulated storm tracks using the open source STORM model (<a href='https://www.nature.com/articles/s41597-020-0381-2' target='_blank'> Bloemendaal et al., 2020 </a>). Using this data, we can make estimates of tropical cyclone probabilities for 1980-2017 and 2015-2050 under RCP8.5 (<a href='https://www.science.org/doi/10.1126/sciadv.abm8438' target='_blank'> Bloemendaal et al., 2022 </a>). We can use these tracks to answer questions such as:

**How often will a community see cyclones of a specific intensity?**

We can count the number of simulated tracks that approach a location within a specific distance. This distance is often set at 100km but can vary depending on the application. 

**How strong will tropical cyclone winds be?**

Wind speeds are highest just outside of the eyewall of a hurricane and generally decrease with distance. The simulated tracks we employ only provide information about the storm location, size and central intensity. To expand each of these tracks into full surface wind and pressure fields, we use the parametric model of <a href='https://journals.ametsoc.org/view/journals/mwre/108/8/1520-0493_1980_108_1212_aamotw_2_0_co_2.xml' target='_blank'>Holland (1980)</a>. We then use the <a href='https://climada-python.readthedocs.io/en/stable/' target='_blank'>CLIMADA</a> Python toolbox to generate these wind fields for thousands of years, allowing us to do a statistical analysis and estimate windspeeds ar 50, 100 and 200 year return periods.

**How high will the storm surge be?**

We can perform numerical ocean simulations to estimate storm surge risk at a location. See our [coastal risk methodology]('../methods/coastal-risk/') for more information.
