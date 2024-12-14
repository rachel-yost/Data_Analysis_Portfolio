## Data Analysis Portfolio
This portfolio was created for the Practical Data Analysis (PHP 2550) class at Brown University. It features projects focusing 
on exploratory data analysis, model building, and simualtion.

### Project 1 - Exploratory Analysis on the Effects of Weather Conditions and Aging on Marathon Performance

Previous studies have found that environmental temperature decreases
marathon performance. Additionally, older adults experience
difficulties with thermoregulation. Using data provided by Dr. Brett
Romano and Dr. Matthew Ely from the Department of Health Sciences at
Providence College, we performed an exploratory data analysis aiming
to examine the effects of increasing age on marathon performance in
men and women; explore the impact of environmental conditions on
marathon performance, and whether the impact differs across age and
gender; and identify the weather parameters that have the largest
impact on marathon performance. We hypothesized that the weather would
have a stronger negative impact on older runners, and that effects
would be similar between men and women. Furthermore,we suspected that
relative humidity, temperature, and solar radiation would have the
strongest impact on runners. Based on the results of my exploratory
data analysis, weather has a stronger impact on runners as age
increases, but effects do not vary significantly by gender.
Furthermore, based on a linear regression and correlations between
race results and weather conditions, we found that relative humidity,
air quality, and solar radiation have the largest impact on marathon
performance. Future research is needed to statistically analyze the
impact of weather, age, and gender on marathon performance.

### Project 2 - Investigating Moderators of Success of Behavioral Activation for Smoking Cessation

Individuals with Major Depressive Disorder (MDD) often struggle with smoking, facing more uncomfortable withdrawal symptoms and a higher probability of relapse that those without MDD. However, they are often are excluded from trials examining possible treatments for smokers. Between 2015 and 2020, researchers at Feinberg School of Medicine conducted a randomized, 2x2 factorial design trial comparing Behavioral Activation Therapy to a standard treatment, and Varenicline to a placebo for smoking cessation in participants with lifetime MDD.

They found that Behavioral Activation Therapy (BA) did not outperform the standard treatment with or without the inclusion of Varenicline. We used the data collected during this study to investigate possible moderators of BA on smoking cessation, as well as the main effects of other covariates. To determine which covariates and interactions were important, we used Lasso for variable selection. We split the data into a training and test set (70/30), and selected lambda using 5-fold cross validation. The full model included the main effects of BA, Varenicline, and all additional covariates, interactions of all variables with BA, and interactions of Varenicline with Black and with an indicator for if the participant is on antidepressants. We evaluated AUC-ROC and model calibration on our test set to check the fit of our model. The model produced an AUC of 0.760 on our training set and 0.715 on our test set. The variables selected by Lasso, other than the treatments-which we chose not to penalize, were Non-Hispanic_White, FTCD score, current MDD, and log(Nicotine Metabolite Ratio). No interactions were selected. The standard treatment slightly outperformed BA, Varenicline outperformed the placebo, non-Hispanic White participants had higher odds of smoking cessation than those who were not non-hispanic White, higher FTCD scores and currently having MDD decreased odds of smoking cessation, and higher log(Nicotine Metabolite Ratio) increased odds of smoking cessation. The results of this analysis suggest that having MDD, a higher dependence on nicotine, being non-Hispanic White, and Nicotine Metabolite Ratio can be predictors of success at quitting smoking, reaffirms that Varenicline is effective, and suggests that BA may be less effective than the standard treatment for smoking cessation.


### Project 3 - Simulation Study to Optimize Cluster Size and Number of Clusters Given Budget Constraints for a Cluster Randomized Controlled Trial

Cluster Randomized Trials are often a useful study design, but can be costly to implement. Outcomes for patients within a cluster are not independent like they are in randomized controlled trials, so researchers must carefully consider their study design. The number of clusters and the size of each cluster must be selected to attain enough statistical power to identify a treatment effect, while also staying within their budgets. It is likely that adding a new cluster to a trial will be more expensive than adding observations to an existing cluster. In this study, we simulate a cluster randomized trial with a fixed budget, and evaluate how the optimal number of clusters and observations per cluster change as data generation parameters are varied. We generate data from a hierarchical model under different values for the within and between cluster variance. We also evaluate how the optimal study design changes based on the relative costs of adding an observation in a new cluster compared to an existing cluster. Data is initially generated following a normal distribution, and then we repeat out simulations on data with a poisson outcome. We found that as the within cluster variance increases relative to the between cluster variance, the optimal number of clusters decreases.
