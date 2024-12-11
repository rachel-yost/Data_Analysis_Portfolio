# Investigating Moderators of Success of Behavioral Activation for Smoking Cessation


### Abstract

Individuals with Major Depressive Disorder (MDD) often struggle with smoking, facing more uncomfortable withdrawal symptoms and a higher probability of relapse that those without MDD. However, they are often are excluded from trials examining possible treatments for smokers. Between 2015 and 2020, researchers at Feinberg School of Medicine conducted a randomized, 2x2 factorial design trial comparing Behavioral Activation Therapy to a standard therapy, and Varenicline to a placebo.

They found that Behavioral Activation Therapy (BA) did not outperform the standard therapy with or without the inclusion of Varenicline. We used the data collected during this study to investigate possible moderators of BA on smoking cessation, as well as the main effects of other covariates. To determine which covariates and interactions were important, we used LASSO for variable selection. We split the data into a training and test set (70/30), and selected lambda using 10-fold cross validation. The full model included the main effects of BA, Varenicline, and all additional covariates, interactions of all variables with BA, and interactions of Varenicline with Black and with an indicator for if the participant is on antidepressants. We evaluated AUC-ROC and model calibration on our test set to check the fit of our model. The variables selected by LASSO were Varenicline, an indicator for Non-Hispanic White, FTCD score, anhedonia, presence of other mental health diagnoses, an indicator for if the participant is currently a smoker, Nicotine Metabolism Ratio (NMR), smoking only menthol cigarettes, BA with income, BA with NMR, BA with smoking only menthol cigarettes, and Varenicline with an indicator for Black. The results of this analysis suggest that the effectiveness of Behavioral Activation Therapy for smoking cessation may vary based on participant characteristics.

### Files
`Project_2.Rmd`: The RMarkdown file which contains the text and code used in my analysis. 

`Project_2.pdf`: The final PDF file containing my report.

### Dependencies

I used R version 4.4.1.

The packages used for this analysis are as follows: 

- Report Generation `knitr` 

- Data Manipulation: `tidyverse`

- Plots and Tables: `corrplot`, `gtsummary`, `gridExtra`, `kableExtra`

- Modeling and Imputation: `glmnet`, `mice`, `pROC`
