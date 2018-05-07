
# Predict the breast cancer recurrence
  Team Member: Yang Hui (1701213132)

  Dataset Source: Breast Cancer Data Set from [UCI](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer)
  
  [The Main ipybn File](https://github.com/Michaelpku/PHBS_TQFML/blob/master/Project/breast-cancer.ipynb)
## Motivation and Goal: 
- The main goal of this project is to find a model to predict the breast cancer recurrence.
- It also tries to identify the top important risk factors in breast cancer recurrence.
- Breast Cancer is one of the most common malignant tumors in women.  It mortality rate ranks first in all women's malignant tumors.
- Since the target dataset is a restricted dataset, there is few machine learning research about it on UCI and Kaggle.

## Dataset description

- This data set includes 201 instances of one class and 85 instances of another class. 
- The instances are described by 9 attributes, some of which are linear and some are nominal. 
- Eight missing values in Node-caps attribute and one missing value in Breast-quadr attribute.
- Attribute Information:
  1. Class: no-recurrence-events, recurrence-events 
  2. Age: 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-89, 90-99. 
  3. Menopause: lt40(before 40), ge40(After 40), premeno(not yet). 
  4. Tumor-size: 0-4, 5-9, 10-14, 15-19, 20-24, 25-29, 30-34, 35-39, 40-44, 45-49, 50-54, 55-59. 
  5. Inv-nodes(the number of nodes invaded): 0-2, 3-5, 6-8, 9-11, 12-14, 15-17, 18-20, 21-23, 24-26, 27-29, 30-32, 33-35, 36-39. 
  6. Node-caps: yes, no. 
  7. Deg-malig(degree of malignant): 1, 2, 3. 
  8. Breast: left, right. 
  9. Breast-quadr(breast quadrant): left-up, left-low, right-up,	right-low, central. 
  10. Irradiat(radiotherapy):	yes, no.

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
- At first, both the training and test accuracies are not so high, 0.762 and 0.786.  In addition, The ROC AUC score is at the similar level, 0.741. 
- Considering the small sample size, K-fold cross-validation is used to check the generalization performance of the model.  As anticipated, the accuracy score is quite volatile, varying from 0.55 to 0.9. The average accuracy score is 0.736. 
- Confusion matrix is also used to examine the predictive power of the model.  The result is quite disappointing.  16 observations were predicted to be negative, while they were positive.
![](https://github.com/Michaelpku/PHBS_TQFML/raw/master/Project/Picture/1.png)
- Tumor_size, Deg_malig, Age, Inv-nodes and Breast are proved to the top five important features or risk factors in Random Forest. Sequential Backward Selection shows similar outcome. The most significant five features are Tumor_size, Deg_malig, Age, Inv_nodes and Node_caps.  Only one feature,Node_caps, differs from the former top five.
![](https://github.com/Michaelpku/PHBS_TQFML/raw/master/Project/Picture/2.png)
- Validation curve is used to see how the training and test accuracy change with hyperparameter C.  Unfortunately, little variance is found on the curve.  The default hyperparameter C=0.1 seems to be better than other alternatives.  Therefore, there is no need to tune the hyperparameter.
![](https://github.com/Michaelpku/PHBS_TQFML/raw/master/Project/Picture/4.png)
- Other algorithms, like Perceptron, SVM, Decision Tree, KNN and Random Forest, are also used to compare with the logistic regression, but none of them showed significant advantage over loggistic regression. Support Vector Machines(rbf) and Perceptron generated highest training accuracy(0.984) and test accuracy(0.798), respectively.  
