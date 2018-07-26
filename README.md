## Exploring Decision Tree Classifiers using [German Credit Data from UCI](https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29)

#### Objective:  Use a decision tree to predict whether a user will default on a credit loan based on quantitive data about the loan and the borrower, using accuracy as  the metric.

A Jupyter notebook was created to perform the analysis using algorithms from scikit-learn.  The analysis roughly follows Chapter 5 of *Machine Learning with R* by Brett Lantz (though of course here we use Python, not R)

The optimized decision tree classifier can predict defaults with about 68-69% accuracy.  This goes up to 69.7% using AdaBoost.

The optimized random forest accuracy is only slightly better at 72%.

The following parameters were explored:

Classifiers:
- Decision Tree
- AdaBoost (with Decision Trees)
- Random Forest

Decision Tree:
- split criteria (gini was best)
- minimum number of samples to allow a split (50 was best)
- maximum tree depth (6 was best)

Random Forest:
- split criteria (gini was best)
- minimum number of samples to allow a split (10 was best)
- maximum tree depth (9 was best)
- number of features to choose from (10 was best)
- number of trees in the forest (50 was best)
