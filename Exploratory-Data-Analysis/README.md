# Exploratory Analysis on the Effects of Weather Conditions and Aging on Marathon Performance


### Abstract

Previous studies have found that environmental temperature decreases marathon performance. Additionally, older adults experience difficulties with thermoregulation. Using data provided by Dr. Brett Romano and Dr. Matthew Ely from the Department of Health Sciences at Providence College, I performed an exploratory data analysis aiming to examine the effects of increasing age on marathon performance in men and women; explore the impact of environmental conditions on marathon performance, and whether the impact differs across age and gender; and identify the weather parameters that have the largest impact on marathon performance. We hypothesized that the weather would have a stronger negative impact on older runners, and that effects would be similar between men and women. Furthermore,we suspected that relative humidity, tempearture, and solar radiation would have the strongest impact on runners. Based on the results of my exploratory data analysis, weather has a stronger impact on runners as age increases, but effects do not vary significantly by gender. Furthermore, based on a linear regression and correlations between race results and weather conditions,we found that relative humidity, air quality, and solar radiation have the largest impact on marathon performance. Future research is needed to further statistically analyze the impact of weather, age, and gender on marathon performance. 

### Files
`Project_1.qmd`: The quarto file which contains the text and code used in my analysis. 

`Project_1.pdf`: The final PDF file containing my report.

### Dependencies

I used R version 4.4.1.

The packages used for this analysis are as follows: 

- Report Generation `knitr` 

- Data Manipulation: `tidyverse`, `lubridate`

- Plots and Tables: `corrplot`, `gtsummary`, `cowplot`, `kableExtra`

- Air Quality Data: `RAQSAPI`
