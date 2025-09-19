---
layout: single
author_profile: false
sidebar:
  nav: "docs"
permalink: /tools/warming-levels/
---

# Warming Levels
*Warming levels are a shorthand for talking about changes in global temperature relative to a baseline period. Common examples are the goals of keeping warming below 1.5°C <a href='https://doi.org/10.1017/9781009157940' target='_blank'>( IPCC, 2018 )</a> or below 2°C <a href='http://unfccc.int/resource/docs/2015/cop21/eng/l09r01.pdf' target='_blank'>( UNFCCC, 2015 )</a> relative to pre-industrial conditions. Warming levels are a useful policy and communication tool as they are easily understood, can help quickly summarize future warming projections, and focus on climate impacts instead of timelines or specific emissions scenarios.*

### Evaluating Warming Level Calculations
Aggregating warming years across models, ensemble members, or scenarios have been used to both increase sample size and account for uncertainty associated with models, natural variability, and emissions pathways, respectively. Aggregating model outputs across multiple models (often referred to as the multi-model mean or ensemble mean) is a common practice in climate science that has been shown to reduce bias relative to using individual models <a href='http://doi.org/10.1098/rsta.2007.2076' target='_blank'>( Tebaldi and Knutti, 2007 )</a>. Aggregating ensemble members, particularly those reflecting different initial conditions, can be helpful to mute the effects of natural internal climate variability <a href='https://doi.org/10.1038/s41558-020-0731-2' target='_blank'>( Deser et al., 2020 )</a>.

Unlike aggregating across models or ensemble members, however, the concept of aggregating warming years, or climate outputs more generally, across scenarios has limited precedent in scientific studies. We evaluated  different approaches for calculating the year when specific global warming levels are reached based on CMIP6 data for user-specified models, ensemble members, and scenarios. For more information, see our methodology <a href='/assets/pdfs/Evaluation of Approaches for Calculating Warming Levels.pdf' target='_blank'>report</a>.

We regularly use a variety of approaches for calculating and aggregating warming levels in our work. You can view the code we use for working with CMIP6 data at specific warming levels in this GitHub repository <a href="https://github.com/woodwellrisk/Warming_levels" target="_blank"><img src="/assets/images/github-icon.png" alt="GitHub icon" style="width:33px;"/></a>. 
