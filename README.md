Heart Failure Predictions
================
Group Green

## Dataset

TODO: INSERT INTRODUCTION FROM PROPOSAL

## Predictor variables

The dataset we chose had 9 categorical variables, including:

-   id

-   gender

-   hypertension

-   heart disease

-   ever married

-   work type

-   residence type

-   smoking status

-   stroke

and 3 quantitative variables, including:

-   age

-   average glucose level

-   bmi

### Selection

We immediately eliminated a few of the variables that we thought were
unlikely to have an effect on stroke likelihood, including id, marriage
status, work type, residence type, and smoking status. For the rest of
the variables, we created a logistical regression model to narrow the
list down further by their p-values, which were shown in the summary
statistics for the model.

A low p-value means that we are closer to rejecting our null hypothesis
that the variable has no effect on stroke likelihood, whereas a high
p-value allows us to assume that the variable has little effect on
stroke likelihood. Based on these statistics, we eliminated gender,
leaving us with age, average glucose level, hypertension, and heart
disease as our four predictor variables.

## Model

We chose to use a logistical regression model as opposed to a linear
regression model because the stroke variable is categorical, meaning
there are only two outcomes: either the individual had a stroke or did
not have a stroke. A logistical regression fits this type of variable
much better than a linear regression.

### Creation

After eliminating predictor variables with a high p-value, we trained a
new logistical regression model using only the remaining predictor
variables on the training data.

### Evaluation

#### Training data

In order to evaluate the performance of the model, we performed 5-fold
cross-validation on the training data and got an accuracy value of
0.9535595 and a ROC area under the curve value of 0.8525241.

The high accuracy value indicates that the model is a good fit to the
data, and the relatively high ROC-AUC value means that the distribution
of the positive curve (individuals who had a stroke) has very little
overlap with the negative curve (individuals wo did not have a stroke).

Visually, when plotting the ROC curve, we can see that the model
attempts to maximize both sensitivity and specificity whenever possible
from the high curve and separation from the mid line.

#### Testing data

After confirming that the model is a good fit for our training data and
can predict stroke likelihood reasonably well, we evaluated the
performance of the model on our training data by creating another
ROC-AUC curve. The AUC value for this curve is 0.813, which is slightly
lower than the AUC value for the training data, but still relatively
high. This indicates that our model is a reasonable fit for the training
data as well and that it can predict stroke likelihood with a reasonably
high degree of accuracy.

## Application

With our newly updated and trained model, we can input a set of
different values for age, average glucose level, hypertension, and heart
disease that represents a single individual and use the predict()
function to determine the likelihood that an individual will have a
stroke. This type of model could be extremely valuable in the healthcare
realm, especially for diseases that occur later in life and are
difficult to predict.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

Soriano, F 2021, Stroke Prediction Dataset, electronic dataset, Kaggle,
viewed 1 April 2021,
<https://www.kaggle.com/fedesoriano/stroke-prediction-dataset>.

## References

Soriano, F 2021, Stroke Prediction Dataset, electronic dataset, Kaggle,
viewed 1 April 2021,
<https://www.kaggle.com/fedesoriano/stroke-prediction-dataset>.
