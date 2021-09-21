---
title: Data
layout: template
order: 3
filename: data
--- 

# Data

|    Description     |             Variable               |     Data Source     |   Use   |
| ------------------ | ---------------------------------- | ------------------- | ------- |
|    Forest Land     |       Hectares of land used        |        UN[^1]       |   EDA   | 
|    National HDI    |              Yearly HDI            |        UN[^1]       |   EDA   |
| Land use in Brazil |            Deforestation           |    MapBiomas[^2].   | OLS/GWR |
|     HDI by state   | indicators of economic wellbeing   | Global Data Lab[^3] | OLS/GWR |

## Fitness for Use

The data from the UN was a simple CSV, but only available at the national level. In this way, while it was good for exploratory data analysis (see [Methods](methods)), it was limiting in what I could do for regression models. Hence, the data from Global Data Lab was used to provide HDI by state for each year.

The data from MapBiomas were more complicated. The project tracks numerous land changes and, as such, this required that I make some critical choices in order to limit the scope of my project, such as eliminating mangrove forests from consideration (see [Further Study](next)). Additionally, the data required extensive scrubbing in order to be used effectively. For the purposes of this study, I forcused on the percent of forest cover per state. However, I am also working on using accumulated hectares of forest loss as a possible variable in a future iteration of this work.

---

[^1]: Datasets from the UN are found at http://data.un.org/Default.aspx These data are in `.csv` format. Forest data report the hectares of land devoted to a particular use in a given year. HDI data reports the aggregate HDI for a given country for each year.

[^2]: The Brazilian Annual Land Use and Land Cover Mapping Project, commonly known as MapBiomas, is a collective project of conservationists and GIS analysts in Brazil interested in gathering data on land use (especially forests) and mapping those changes over time. Data is made available for further analysis. The English-language statistics page can be [found here](https://mapbiomas.org/en/estatisticas?cama_set_language=en)

[^3]: The [Global Data Lab](https://globaldatalab.org) is a project of the Institute for Management Research at Radboud University in the Netherlands. Their datasets include measures of HDI at sub-national levels.
