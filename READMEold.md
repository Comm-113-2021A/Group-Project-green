# Group Project

yl: I like this idea, in general, but I think we can make it more interesting with the tools from the next few weeks. Rather than simply looking at the correlations in this dataset, how about a project where you create a machine learning model to predict who is most likely to have heart problems? I.e., can you work on a personalized medicine project? Take some background info and figure out the risk that they get heart disease?

The heart failure dataset is a bit small, but I think there are lots of other options here including  aheart disease dataset: 
https://archive.ics.uci.edu/ml/datasets.php?format=&task=&att=&area=life&numAtt=&numIns=&type=&sort=nameUp&view=table

One issue with this proposal is that you didn't really do any preliminary data analysis related to your questions. I like that you used the codebook package, but you didn't really do anything beyond that. 

9/10.

### Section 1: Introduction  
Our group chose to use the "Heart Failure Predition" dataset (https://www.kaggle.com/andrewmvd/heart-failure-clinical-data) from
a study published in *BMC Medical Informatics and Decision Making* by Davide Chicco & Giuseppe Jurman to answer our research question, which is "Between the
blood levels of platelets, serum creatinine, and serum sodium, which has the
greatest impact on the likelihood of death for a heart failure patient?"

Chicco & Jurman observed 299 patients with heart failure in 2015, and collected data on their age, sex, ejection fraction percentage, smoking status, whether they had anaemia, hypertension, or diabetes, CPK/platelet/serum creatinine/serum sodium levels, follow-up period after intial observation, and death event.

### Section 2: Data  
See READMEdata file in /data folder. Preliminary exploratory data analysis is included in the codebook.

### Section 3: Data Analysis Plan  
*Explanatory variables:* platelet level, serum creatinine level, and serum sodium level

*Response variable:* death outcome

We hope to create some visual representation of the correlation between death event and each one of the explanatory variables in order to determine which one has the greatest effect on death outcome. Specifically, we plan to create a dot plot or line graph and calculate the correlation coefficient between each of the variables and death outcome. However, we are currently searching for a better way to represent the data visually given that the death outcome is a boolean value and a dot plot/line graph may not be the best way to illustrate this.


