:# Recurrence probability of breast cancer
Team Member: Yang Hui (1701213132)

Dataset Source: Breast Cancer Data Set from UCI, https://archive.ics.uci.edu/ml/datasets/Breast+Cancer
## Motivation: 
- The main goal of this project is to predict the probability of surviving at least one year for HCC patients.

- It is a real clinical data of 165 patients diagnosed with HCC collected at a University Hospital in Portugal.
## Dataset description

- This data set includes 201 instances of one class and 85 instances of another class. 
- The instances are described by 9 attributes, some of which are linear and some are nominal. 
- Attribute Information:
  1. Class: no-recurrence-events, recurrence-events 
  2. age: 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80-89, 90-99. 
  3. menopause: lt40, ge40, premeno. 
  4. tumor-size: 0-4, 5-9, 10-14, 15-19, 20-24, 25-29, 30-34, 35-39, 40-44, 45-49, 50-54, 55-59. 
  5. inv-nodes: 0-2, 3-5, 6-8, 9-11, 12-14, 15-17, 18-20, 21-23, 24-26, 27-29, 30-32, 33-35, 36-39. 
  6. node-caps: yes, no. 
  7. deg-malig: 1, 2, 3. 
  8. breast: left, right. 
  9. breast-quad: left-up, left-low, right-up,	right-low, central. 
  10. irradiat:	yes, no.



## Methodology
- Import data and check
- Drop samples containing missing value
- Preprocess:
  1.Encode catagories
  2.Split data into training set and test set
  3.
- 
## Result and Conclusion
- After getting the overall classification effect, the main algorithm logistic regression with L2 regularization will be used in this project.
-This final model will be used to predict the probability of surviving at least one year for HCC patients.
