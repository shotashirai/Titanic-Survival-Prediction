# Kaggle titanic analysis
Jupyter notebook in Python to analyse titanic passenger data from Kaggle.

## Project Summary
**Situation**  
Titanic sank after colliding with an iceberg on 15th April 1912, resulting in the death of 1502 out of 2224 passengers and crew. Although there was a luck element to survive in this incident, it seems that some groups of people were more likely to survive than others. This project aims to find key elements related to survived groups and predict who can survive in the Titanic shipwreck.  
  
**Action and Goal**  
Using the passenger data provided by Kaggle, exploratory data analysis (EDA) and model deployment are implemented by using Python and Jupyter notebook. The goal is to build a predictive model that answers the question: what kind of people/groups is more likely to survive? Since the output from the model is expected to be binary (1:survived or 0:not survived), a binary model is needed to be built by exploring classification algorithms such as decision tree, random forest, support vector machine (SVM) and a neural network. The deployed model is evaluated by cross-validation and the result from the model is submitted to the Kaggle leaderboard.

## Data
"Titanic passenger dataset" in Kaggle is used. This dataset is publically available (https://www.kaggle.com/c/titanic/data).

## Methodology
### Exploratory Data Analysis (EDA) / Data enginnering
Initial exploration of the training data and test data has been done on Jupyter notebook (TitanicSurvivalPrediction_EDA_Model.ipynb) using **pandas** and **pandas_profiling**. The pandas_plofiling generates ProfileReport describe statistics (data type, missing values, histogram, etc...) of the data on an interactive HTML report. To visualise the detail of the data, **Plotly** and **Seaborn** are used. At this stage, missing data is also interpolated.
  
### Classification model
To classify passengers into survived and not survived, binary models are built using (**Linear regression, Logistic Regression, Extra Trees, Random Forest, Gradient Boosting, neural network**). To build the models, **scikit-learn** and **Keras** were used. The results of the classifications were evaluated using **k-fold cross-validation**. 

## Results
The best result among the models with an accuracy of 82% using Random Forest achieved a submission position within **the top 8%** of the Kaggle Submission Leaderboard (~33,000 teams). The analysis is shown in the notebook (TitanicSurvivalPrediction_EDA_Model.ipynb)
