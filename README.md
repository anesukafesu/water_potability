# Assignment to build a Machine Learning Model to predict Water Potability

Team Members and Roles
1. Anesu Kafesu (Data Handling and Error Analysis)
2. Davy Nkurunziza (Vanilla Model Implementation)
3. Prince Ndanyuzwe (L1 Model Implementation)
4. Ken Kalisa Ganza (L2 Model Implementation)

# Data Handling

## Activity
For Task 1, we cleaned and explored the data to find correlations between potability and other features. We used heatmaps and scatter plots to visualise the correlations.

## Findings
We found that there was little to no correlation between the different features and the data. This led us to conclude that perhaps individual features do not contribute to the data, but rather, combinations of features(super-features). Therefore, we decided to implement a deep neural network in the steps that followed.

# Vanilla Model
## Activity

## Findings

# L1 Regularization
## Activity

## Findings


# L2 Regularization
## Activity
In this task we added L2(Ridge) Regularization to dense layers to avoid overfitting. We also added Early stopping primarily monitoring the validation loss each 10 epochs. Among others we used Adam optimization and Binary cross entropy since this was a binary classification model. In the process of early stopping we used three values 5, 10 and 12.

## Findings
The model accuracy slightly increased as we increased the value to 10 but once again decreased after increasing to 12, indicating that overfitting had started. Leading to an assumption that 10 is the ideal patience value. Overall, the model performed well, balancing both regularisation and early stopping to optimise its accuracy and prevent overfitting.

# Error Analysis
## Activity
We evaluated the models using 3 metrics, loss, accuracy and precision. Precision was the most important indicator for model performance for us and this is how the different models fared:

## Findings
### Losses
Vanilla Model: 0.6243797540664673
L1 Model: 0.6486924886703491
L2 Model: 0.635040283203125

### Accuracies
Vanilla Model: 0.6848635077476501
L1 Model: 0.6898263096809387
L2 Model: 0.6823821067810059

### Precision
Vanilla Model: 0.6666667
L1 Model: 0.7196262
L2 Model: 0.72

Therefore, the L2 model was the best-performing model with an accuracy of 72%.
