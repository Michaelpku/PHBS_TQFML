Repository name：Michaelpku/PHBS_TQFML/Project
Team Member: Yang Hui
Data set: HCC Survival Data Set from UCI.  https://archive.ics.uci.edu/ml/datasets/HCC+Survival
Brief plan of the project: The main goal of this project is to predict the probability of surviving at least one year for HCC patients.
It is a real clinical data of 165 patients diagnosed with HCC collected at a University Hospital in Portugal.
This dataset contais several demographic, risk factors, laboratory and overall survival features of 165 real patients diagnosed with HCC.
There are 23 quantitative variables, and 26 qualitative variables in these features.
After being preprocessed, all left features will be selected as the input X according to their importance and completeness.
Survival feature will be the target variable y. 
Several algorithms will be used to fit and test these models to check whether it needs further feature extraction or not.
After getting the overall classification effect, the main algorithm logistic regression with L2 regularization will be used in this project.
Through changing the regularization parameter C, we get the most five improtant features and the final model.
This final model will be used to predict the probability of surviving at least one year for HCC patients.
