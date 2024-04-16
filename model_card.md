# Model Card

## Model Description

**Input:** data/car_insurance_claim.csv

**Output:** Binary output wheather or not cliam occured

**Model Architecture:** 
- Logistic regression is a supervised learning algorithm for binary classification tasks. It works by modeling the relationship between the independent variables (predictors) and the dependent variable (target) using a sigmoid function, which outputs a probability between 0 and 1
- XGBClassifier implements an optimized version of the gradient boosting algorithm, which is an ensemble learning method that builds a strong predictive model by combining multiple weak models, typically decision trees, in a sequential manner

## Performance

Below is the summary of 3 models used and performance metrrcs used on test data set.  

| Classifier                 | F1_score | Accuracy score |
|----------------------------|----------|----------------|
| LogisticRegression         | 0.77249  | 0.7933         |
| GradientBoostingClassifier | 0.77545  | 0.79622        |
| XGBClassifier              | 0.77574  | 0.79185        |

## Limitations

model couldn't be tuned for min_samples_splits, min_samples_leafs, max_features.

## Trade-offs

Since data was imbalance therefore f1_score was more focused performance indicators and accuracy was not main focus 
