# Uber-Fares-Prediction
          
  - [Overview](#overview)
    - [Dataset Descrption](#dataset-descrption)
  - [Best Model selection](#best-model-selection)
    - [Best parametes](#best-parametes)
  - [Technologies Used](#technologies-used)


## Overview
The Uber price dataset is a dataset that contains information about Uber prices in different regions. This group includes information such as the time and date of the trip, the start and destination location, the distance and duration of the trip, and the fare paid.
The Uber Fares dataset is used to analyze trip patterns, predict trip costs, and understand user behavior. This data can be used to improve transportation service, develop pricing strategies, and improve user experience.
The Uber Fares dataset is a valuable collection for data scientists and data analysts to understand rider behavior, predict demand patterns, and analyze billing. Advanced data analysis techniques such as machine learning and data mining can be used to leverage this combination to discover new trends and patterns.
It is important to consider privacy and security when using Uber Fares data collection, and you should ensure that use complies with privacy policies and applicable local laws.

<img src = "https://github.com/ahmedsaeed620/CodeClauseInternship_Uber-Fares-Prediction/blob/main/Images/TAL-uber-screen-car-UBERHOLIDAY1122-50314d4bd42e4316bec881419eab2d3d.jpg" width = 450 height = 200/> <img src = "https://github.com/ahmedsaeed620/CodeClauseInternship_Uber-Fares-Prediction/blob/main/Images/download.jpg" width = 450 height = 200/>
<img src = "https://github.com/ahmedsaeed620/CodeClauseInternship_Uber-Fares-Prediction/blob/main/Images/uber.webp" width = 450 height = 200/> <img src = "https://github.com/ahmedsaeed620/CodeClauseInternship_Uber-Fares-Prediction/blob/main/Images/Uber-driver-holds-smartphone-in-car.webp" width = 450 height = 200/>

### Dataset Descrption

Dataset used here is from a [Kaggle Datast ](https://www.kaggle.com/datasets/yasserh/uber-fares-dataset). 

* Size of Dataset set: 200000 records
  
* **Features**: 
  - key : A unique identifier for each trip. 
  - fare_amount: The cost of each trip in usd. 
  - pickup_datetime : Date and time when the meter was engaged. 
  - passenger_count : The number of passengers in the vehicle (driver entered value). 
  - pickup_longitude : The longitude where the meter was engaged. 
  - pickup_latitude : The latitude where the meter was engaged. 
  - dropoff_longitude : The longitude where the meter was disengaged. 
  - dropoff_latitude : The latitude where the meter was disengaged. 
  
## Best Model selection

The data is trained on Linear Regression, Ridge, PolynomialFeatures , Decision Tree Regressor, Random Forest Regressor, VotingRegressor, BaggingRegressor, AdaBoost Regressor, GradientBoostingRegressor, and XGBoost. GradientBoostingRegressor turned out to be the best model with accuracy= 84.62.


### Best parametes

``` python
{'Model_fit__n_estimators': 200,
  'Model_fit__max_depth': 5 }
```

## Technologies Used

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org)
[![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org) 
[![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com) 
[![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)


Link My accaount in Kaggle : [Ahmed elsaied](https://www.kaggle.com/ahmedsaied3122)

Link My notebook in Kaggle : [Uber Fares Prediction](https://www.kaggle.com/code/ahmedsaied3122/uber-fares-prediction/notebook)







