---
title: Methods
layout: template
order: 4
filename: methods
---

# Methods

The first methods employed were exploratory. First I plotted the changes over time for both the national forest cover (in hectartes) and the national HDI (these data came from the UN). As you can see, forests are steadily decreasing while HDI is steadily increasing. Once I calculated the percentage of forest cover per state (by using numbers from MapBiomas), I was also able to plot a histogram of forest cover. This shows that the majority of states are less forested but a few are incredibly forested. Again, this leads me to believe that spatial analysis would be worthwhile. The histogram of state-level HDI also piqued my curiosity, as I wondered if the few states with lower HDI were the same few with greater forest cover.

<div class="flourish-embed" data-src="story/837076"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

From here, I ran fairly standard exploratory spatial data analysis. My Global Moran's *I* was only a positive 0.12, meaning there was slight spatial autocorrelation. However, there was no spatial autocorrelation in the residuals. Spatial models (SLM and SEM) did not fit better than a non-spatial OLS regression. However, geographically-weighted regression (GWR) shows some promise, at least fitting better than OLS. Further GWR analysis will hopefully clarify the patterns in the data (see also [Further Study](next) for a note on other variables to consider).

While I did not closely use remote sensing data for this project yet, I did have a chance to view some photo data.

<div class="flourish-embed flourish-photo-slider" data-src="visualisation/5973903"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

In short, these data show change over time -- even evident in the satellite images. Correlation measures show that there's roughly a 20% correlation between the percent of forest cover and the HDI. Typical spatial regression models, however, don't produce clear results. As I continued to dig in the data I mapped my findings and formullated several hypotheses.

**Next:** [Findings](findings)
