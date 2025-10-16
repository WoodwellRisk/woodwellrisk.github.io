---
template: main.html

hide:
  - toc
  - path
---

# Flooding
*Flooding, both in riverine flood plain and at the coast, poses one of the most significant natural threats to property and life. Under future climate, changes in precipition patterns, storm events and sea level will also impact where and when dangerous flooding will occur. Our suite of flooding tools and datasets allows us to assess flood risk both today and in the future.*

## Flood Modelling
Coastal and inland flood risk is simulated using the LISFLOOD-FP flood model (<a href="https://gmd.copernicus.org/articles/16/2391/2023/" target="_blank"> Sharifian et al., 2022 </a>). LISFLOOD-FP takes into account streamflow, rainfall, storm surge, land cover, and soil infiltration to estimate maximum flood depth. Dynamics between surface flow and stormwater systems can be modeled using a coupling framework between LISFLOOD-FP and Stormwater Management Model <a href="https://www.epa.gov/water-research/storm-water-management-model-swmm" target="_blank">( SWMM )</a> that was developed in-house. We are able to simulate flooding at high spatial resolutions ranging from less than 5 meters to 30 meters.

## Sea Level Rise Inundation Extent
Sea level rise inundation is mapped globally at a 30-meter resolution using our internally developed global DEM (see [DiluviumDEM](http://127.0.0.1:4000/risks/flooding/#diluviumdem-enhanced-accuracy-in-global-coastal-digital-elevation-models-) below) or local DEMs where available. Local sea level rise projections are from the <a href="https://sealevel.nasa.gov/data_tools/17" target="_blank">NASA IPCC AR6</a> dataset <a href="https://doi.org/10.1017/9781009157896.011" target="_blank">( Fox-Kemper et al., 2021 )</a>. These projections take into account ocean thermal expansion, glacial and ice cap melting, and subsidence. The coastal water levels of the annual flood (1-year return period) are added to the sea level rise projections to represent the highest yearly water level around the globe (<a href="https://www.frontiersin.org/articles/10.3389/fmars.2020.00263/full" target="_blank"> Muis et al., 2020 </a>). Finally, a bathtub approach in conjunction with a connected components analysis is used to estimate future annual inundation from sea level rise.

## Storm Surge Inundation <a href="https://github.com/WoodwellRisk/CRisk" target="_blank">:simple-github:{ .md }</a>

Our Coastal Risk Framework uses state of the art numerical and statistical modelling techniques to estimate coastal storm surge (due to tropical cyclones) return periods anywhere in the world. The framework consists of synthetic tropical cyclones (as in [Tropical Cyclones](/risks/tropical-cyclones/)), statistical hurricane models, a numerical ocean model (ROMS) and our LISFLOOD flood model configuration (see [Flooding](/risks/flooding/)). The final analysis is coastal storm surge return levels and flood inundation extents for coastal communities.

For more information, see our more in depth [methodology](/methods/coastal-risk/).

*The development of this framework was presented at the international Ocean Sciences Meeting 2024 in New Orleans. You can view the poster by clicking here:* <a href="https://doi.org/10.5281/zenodo.10737286" target="_blank">![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10737286.svg)<a>

## DiluviumDEM: Enhanced accuracy in global coastal digital elevation models <a href="https://github.com/ddusseau/DiluviumDEM" target="_blank">:simple-github:{ .md }</a>


The most important component of any flood analysis is the accuracy of the elevation used in the model -- often called a Digital Elevation Model (DEM). Where possible, we use locally sourced, high resolution DEMs in our models. However, when this data is not available, we use Diluvium: our state-of-the-art, machine learning enhanced DEM, as developed by <a href='https://www.sciencedirect.com/science/article/pii/S0034425723003632?via%3Dihub' target='_blank'>Dusseau et al. (2023)</a>.
