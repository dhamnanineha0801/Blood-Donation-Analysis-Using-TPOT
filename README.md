# Blood-Donation-Analysis-Using-TPOT

![Figure 1-1](https://github.com/dhamnanineha0801/Blood-Donation-Analysis-Using-TPOT/blob/main/images/tpot-logo.jpg "Figure 1-1")


## Project Summary

The project aims to predict whether people who've previously donated blood are likely to return to donate blood at a future date. This is important because blood is sued in may serious medical procedures and could be the factor between life or death for a patient.

## About TPOT

TPOT stands for Tree-based Pipeline Optimization Tool. Consider TPOT your Data Science Assistant. TPOT is a Python Automated Machine Learning tool that optimizes machine learning pipelines using genetic programming.

TPOT will automate the most tedious part of machine learning by intelligently exploring thousands of possible pipelines to find the best one for your data.

![Figure 1-1](https://github.com/dhamnanineha0801/Blood-Donation-Analysis-Using-TPOT/blob/main/images/tpot-ml-pipeline.png "Figure 1-1")

## Data Preparation, Data cleaning and Model Selection

**Pipeline instructions**
- Data cleaning  and preprocessing:
    There were no missing or duplicate values in the dataset and all the entries were already of the integer datatype. The dataset also contained no imbalances.

- Data preparation:
    The data was split into training and testing sets, 75% for the training set and 25% for the test set. The column "monetary" which contained the volume of blood donated was skewed so it had to be normalised.
    
- Model selection:
    We tested the models that were used in the research papers that we reviewed; BernoulliNB, SVM, Decision Trees and ANN for their accuracies on our dataset. Out of the four SVM performed best with an accuracy of 77.54%.
    Then we implemented TPOT autoML and got the Best pipeline: LogisticRegression(RobustScaler(input_matrix), C=25.0, dual=False, penalty=l2) which had an accuracy of 78.57%.
    Using this best pipeline suggestion from TPOT, we implemented our own Logistic regression model and got an accuracy score of 78.9%

**The Data**
The dataset we will be working on is from a mobile blood donation vehicle in Taiwan. The Blood Transfusion Service Center drives to different places and collects blood as part of a blood drive. The dataset includes the recency (how recent the person's last blood donation was), frequency (how many times the person has donated blood), monetary (the volume of blood donated), the time (the duration from the first time they donated to the last time they donated), and whether or not they donated in March 2007.
The last column will serve as the target.



### Prerequisites

- TPOT
- Sklearn
- Matplotlib


### Datasets
Dataset is located in the data folder


### Code

The attached .ipynb file has the executed code





