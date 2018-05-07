
# Probability of breast cancer recurrence
  Team Member: Yang Hui (1701213132)

  Dataset Source: Breast Cancer Data Set from UCI, https://archive.ics.uci.edu/ml/datasets/Breast+Cancer
## Motivation and Goal: 
- The main goal of this project is to predict the probability of breast cancer recurrence.
- Breast Cancer is one of the most common malignant tumors in women.  It mortality rate ranks first in all women's malignant tumors.
- Since the target dataset is a restricted dataset, there is few machine learning research about it on UCI and Kaggle.

## Dataset description

- This data set includes 201 instances of one class and 85 instances of another class. 
- The instances are described by 9 attributes, some of which are linear and some are nominal. 
- Eight missing values in Node-caps attribute and one missing value in Breast-quadr attribute.
- Attribute Information:
  1. Class: no-recurrence-events, recurrence-events 
  2. Age: 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-89, 90-99. 
  3. Menopause: lt40, ge40, premeno. 
  4. Tumor-size: 0-4, 5-9, 10-14, 15-19, 20-24, 25-29, 30-34, 35-39, 40-44, 45-49, 50-54, 55-59. 
  5. Inv-nodes: 0-2, 3-5, 6-8, 9-11, 12-14, 15-17, 18-20, 21-23, 24-26, 27-29, 30-32, 33-35, 36-39. 
  6. Node-caps: yes, no. 
  7. Deg-malig: 1, 2, 3. 
  8. Breast: left, right. 
  9. Breast-quadr: left-up, left-low, right-up,	right-low, central. 
  10. Irradiat:	yes, no.

## Methodology
- The main algorithm used in this project is logistic regression with L2 regularization(parameter c=0.1).
- Import data and check
- Preprocess:
  1. Drop samples
  2. Encode catagories
  3. Recheck dataset
  4. Split the dataset
- Logistic Regression and Metrics
- Assessing Feature Importance
- Tuning Hyperparameter with validation curves
- Check the result with other algorithms

## Result and Conclusion
- 
-
