# Kaggle titanic analysis
Python script/Jupyter notebook to analyse titanic data from Kaggle.

## Data
For this analysis, "Titanic passenger dataset in Kaggle is used. This dataset is publically avaialble (https://www.kaggle.com/c/titanic/data).

## Exploratory Data Analysis (EDA) / Data enginnering
Initial exploration of the training data and test data has been done on Jupyter notebook (TitanicSurvivalPrediction_EDA_Model.ipynb) using **pandas** and **pandas_profiling**. The pandas_plofiling provides ProfileReport including some metrics and correlations. To visualise the detail of the data, **Plotly** and **Seaborn** are used. At this stage, missing data is also interpolated.
  
## Modeling / Classification
To classify passengers into survived and not survived, various models (**Linear regression, Logistic Regression, Decision Tree, Random Forest, Gradient Boosting**) were used and the results were evaluated using **k-fold cross-validation**. The best result among the models with an accuracy of 82% using Random Forest achieved a submission position within the top 8% of the Kaggle Submission Leaderboard (~38,000 teams).  
The analysis is shown in the notebook (TitanicSurvivalPrediction_EDA_Model.ipynb.ipynb)
