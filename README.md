# Recurrence probability of breast cancer
Team Member: Yang Hui (1701213132)

Dataset Source: Breast Cancer Data Set from UCI, https://archive.ics.uci.edu/ml/datasets/Breast+Cancer
## Motivation: 
- The main goal of this project is to predict the probability of surviving at least one year for HCC patients.


- It is a real clinical data of 165 patients diagnosed with HCC collected at a University Hospital in Portugal.
This dataset contais several demographic, risk factors, laboratory and overall survival features of 165 real patients diagnosed with HCC.
There are 23 quantitative variables, and 26 qualitative variables in these features.
## Dataset description

- After being preprocessed, all left features will be selected as the input X according to their importance and completeness.
- Survival feature will be the target variable y. 

## Methodology
- Several algorithms will be used to fit and test these models to check whether it needs further feature reduction and extraction or not.

## Result and Conclusion
- After getting the overall classification effect, the main algorithm logistic regression with L2 regularization will be used in this project.
-This final model will be used to predict the probability of surviving at least one year for HCC patients.
