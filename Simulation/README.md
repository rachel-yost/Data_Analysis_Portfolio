# Project-3-PDA

# Simulation Study to Optimize Cluster Size and Number of Clusters Given Budget Constraints for a Cluster Randomized Controlled Trial


### Abstract

Cluster Randomized Trials are often a useful study design, but can be
costly to implement. Outcomes for patients within a cluster are not
independent like they are in randomized controlled trials, so
researchers must carefully consider their study design. The number of
clusters and the size of each cluster must be selected to attain
enough statistical power to identify a treatment effect, while also
staying within their budgets. It is likely that adding a new cluster
to a trial will be more expensive than adding observations to an
existing cluster. In this study, we simulate a cluster randomized
trial with a fixed budget, and evaluate how the optimal number of
clusters and observations per cluster change as data generation
parameters are varied. We generate data from a hierarchical model
under different values for the within and between cluster variance. We
also evaluate how the optimal study design changes based on the
relative costs of adding an observation in a new cluster compared to
an existing cluster. Data is initially generated following a normal
distribution, and then we repeat out simulations on data with a
poisson outcome. We found that as the within cluster variance
increases relative to the between cluster variance, the optimal number
of clusters decreases.

### Files
`Project3.qmd`: The qmd file which contains the text and code used in my analysis. 

`Project3.pdf`: The final PDF file containing my report.

`Sim_Results`: Folder containing the csv files from our simulations

### Dependencies

I used R version 4.4.1.

The packages used for this analysis are as follows: 

- Report Generation `knitr` 

- Data Manipulation: `tidyverse`

- Plots and Tables: `ggplot2`, `gridExtra`, `kableExtra`

- Modeling and Imputation: `lme4`
