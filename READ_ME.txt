#################################################################################

                                    READ ME

#################################################################################

We performed classification on the Gisette Dataset in 4 different ways using 5 different models and saved them as separate run-able codes.

#################################################################################

FIVE MODELS:

1. Logistic Regression
2. Linear Kernel SVM
3. 2nd Degree Polynomial Kernel SVM
4. 3rd Degree Polynomial Kernel SVM
5. 4th Degree Polynomial Kernel SVM

#################################################################################

FOUR DATASETS:

1. The Whole Dataset

Run "whole_data_run.ipynb" file to get results of all five models on the whole non-reduced dataset.

2. Feature Mean Value Reduced Dataset

In this approach, we separated the training dataset into two 3000 x 5000 datasets based on their labels either 1 or -1. Then we calculated mean across the features to get two 1 x 5000 datasets that stored the average values. Afterwards, we calculated the differene between these mean values stored in the two datasets individually for each feature. Then filtered down our features using the absolute value of this difference to be at least 50.

Run "feature_mean_reduced_data_run.ipynb" file to gain a better understanding of our approach and to get results of all five models on this reduced dataset.

3. Correlation & Multi-Collinearity Reduced Dataset

Here we calculated correlation of each feature to the target value and kept a feature only if it was at least in 15% correlation with the target.
Then we calculated Variance Inflation Factor of the remaining dataset and kept a feature only if it had VIF less than 10.

Run "correlation_multicollinearity_reduced_data_run.ipynb" file to gain a better understanding of our approach and to get results of all five models on this reduced dataset.

4. Principal Component Analysis Reduced Dataset

We performed PCA on our dataset and reduced the features to principal components capturing at least 85% variability of the dataset.

Run "PCA_reduced_data_run.ipynb" file to gain a better understanding of our approach and to get results of all five models on this reduced dataset.

##################################################################################################################################################################

     Thank You and further clarifications will be provided when presenting

##################################################################################################################################################################










