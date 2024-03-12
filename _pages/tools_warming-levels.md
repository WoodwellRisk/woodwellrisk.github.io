---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /tools_warming-levels/
---

# Warming Levels
*Warming levels are a shorthand for talking about changes in global temperature relative to a baseline period. Common examples are the goals of keeping warming below 1.5°C [(IPCC, 2018)](https://doi.org/10.1017/9781009157940) or below 2°C [(UNFCCC, 2015)](http://unfccc.int/resource/docs/2015/cop21/eng/l09r01.pdf) relative to pre-industrial conditions. Warming levels are a useful policy and communication tool as they are easily understood, can help quickly summarize future warming projections, and focus on climate impacts instead of timelines or specific emissions scenarios.*

### Evalulating Warming Level Calculations [![GH Logo](/assets/images/github-mark.png)](https://github.com/WoodwellRisk/Warming_levels)
Aggregating warming years across models, ensemble members, or scenarios have been used to both increase sample size and account for uncertainty associated with models, natural variability, and emissions pathways, respectively. Aggregating model outputs across multiple models (often referred to as the multi-model mean or ensemble mean) is a common practice in climate science that has been shown to reduce bias relative to using individual models [(Tebaldi and Knutti, 2007)](http://doi.org/10.1098/rsta.2007.2076). Aggregating ensemble members, particularly those reflecting different initial conditions, can be helpful to mute the effects of natural internal climate variability [(Deser et al., 2020)](https://doi.org/10.1038/s41558-020-0731-2).

Unlike aggregating across models or ensemble members, however, the concept of aggregating warming years, or climate outputs more generally, across scenarios has limited precedent in scientific studies. This analysis evaluates different approaches for calculating the year when specific global warming levels are reached based on CMIP6 data for user-specified models, ensemble members, and scenarios.

