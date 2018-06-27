# donorchoose.org-fully-funded-projects

The main noteboook includes all the codes, results, graphs and interpretations from data explorations, to data processing, to features generations, to temporal validations, and evaluations. 

The appendix notebook contains all the progress work of data explorations. 

The project is derived from KDD 2014, for more details please check https://www.kaggle.com/c/kdd-cup-2014-predicting-excitement-at-donors-choose. The data is also pulled from this webpage. 



#Project Descriptions:

Task: 
The goal is to predict, at posting time of a project, if a project will not get fully funded so we can intervene and help them improve the project listing.


Methods:
Use all the classifiers - I’d recommend at least having Logistic Regression, K-Nearest Neighbor, Decision Trees, SVM, Random Forests, Boosting, and Bagging. The code should have a parameter for running one or more of these classifiers and your analysis should run all of them.

Experiment with different parameters for these classifiers (different values of k for example, as well as parameters that other classifiers have). You should look at the sklearn documentation to see what parameter each classifier can take and what the default values sklearn selects.

Add additional evaluation metrics that we've covered in class to the pipeline (accuracy, precision at different levels, recall at different levels, F1, area under curve, and precision-recall curves).

Create temporal validation function in your pipeline that can create training and test sets over time. You can choose the length of these splits based on analyzing the data. For example, the test sets could be six months long and the training sets could be all the data before each test set. Please use train test windows over time and produce results for each test set.

train 2006-2009 test 2010 and so on...


#Output: 
1. Documented Code in a github repository

2. The code should produce a table with results across train test splits over time and performance metrics (baseline, precision and recall at different thresholds 1%, 2%, 5%, 10%, 20%, 30%, 50% and AUC_ROC)

3. Report: You should also write a short report (6-8 pages) that reads like a project report. It should describe the data, describe the problem, compare the performance of the different classifiers across all the metrics . Which classifier does better on which metrics? How do the results change over time? What would be your recommendation to someone who's working on this model on which model to select to implement? 

The report should not be a list of graphs and numbers. It needs to explain to a policy audience the implications of your analysis and your recommendations as a memo you would send to a business/policy audience.
