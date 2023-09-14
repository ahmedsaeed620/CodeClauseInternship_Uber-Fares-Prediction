# Uber-Fares-Prediction
          
  - [Overview](#overview)
    - [Dataset Descrption](#dataset-descrption)
  - [EDA](#EDA-selection)
  - [Best Model selection](#best-model-selection)
    - [Best parametes](#best-parametes)
  - [Technologies Used](#technologies-used)


## Overview
The Uber price dataset is a dataset that contains information about Uber prices in different regions. This group includes information such as the time and date of the trip, the start and destination location, the distance and duration of the trip, and the fare paid.
The Uber Fares dataset is used to analyze trip patterns, predict trip costs, and understand user behavior. This data can be used to improve transportation service, develop pricing strategies, and improve user experience.
The Uber Fares dataset is a valuable collection for data scientists and data analysts to understand rider behavior, predict demand patterns, and analyze billing. Advanced data analysis techniques such as machine learning and data mining can be used to leverage this combination to discover new trends and patterns.
It is important to consider privacy and security when using Uber Fares data collection, and you should ensure that use complies with privacy policies and applicable local laws.

<img src = "https://github.com/ahmedsaeed620/Price-prediction-of-used-cars/blob/main/images/a.jpg" width = 350 height = 200/> <img src = "https://github.com/ahmedsaeed620/Price-prediction-of-used-cars/blob/main/images/s.jpg" width = 350 height = 200/>
<img src = "https://github.com/ahmedsaeed620/Price-prediction-of-used-cars/blob/main/images/i.jpg" width = 350 height = 200/> <img src = "https://github.com/ahmedsaeed620/Price-prediction-of-used-cars/blob/main/images/d.jpg" width = 350 height = 200/>

### Dataset Descrption

Dataset used here is from a [Kaggle](https://www.kaggle.com/datasets/avikasliwal/used-cars-price-prediction). The dataset set contains features like Location, Manufacture details, car features such as Fuel type, Engine, and usage parameters. Below is the app in Working condition.

* Size of training set: 6,019 records
  
* **Features**: 
  - Name: The brand and model of the car. 
  - Location: The location in which the car is being sold or is available for purchase. 
  - Year: The year or edition of the model. 
  - Kilometers_Driven: The total kilometres driven in the car by the previous owner(s) in KM. 
  - Fuel_Type: The type of fuel used by the car. Transmission: The type of transmission used by the car. 
  - Owner_Type: Whether the ownership is Firsthand, Second hand or other. 
  - Mileage: The standard mileage offered by the car company in kmpl or km/kg 
  - Engine: The displacement volume of the engine in cc. 
  - Power: The maximum power of the engine in bhp. 
  - Seats: The number of seats in the car. 
  - New_Price: The price of a new car of the same model. 
  - Price: The price of the used car in INR Lakhs.
 
##  EDA
In this section of the project, the data is explored to see the patterns and trends and observe interesting insights. Below are some interesting observations generated.

- ```New_Price``` feature dropped due to significant missing values. 
- ```Name``` column split into ```Brand``` feature.
- Continuos variables including target feature are Log transformed to make their distribution symetrical.
-  ```Kilometers_Driven``` and ```Mileage``` are multiplied together to form new feature as this interaction show high correlation with target feature ```price```.
- ```Brand```, ```Fuel_Type```, ```Transmission``` and ```Location``` are encoded using **bainary encoding** as they have lot of categories.
- ```Owner_Type``` is ```ordinal_encoder```.


## Best Model selection

The data is trained on Linear Regression, Ridge, SVR, Decision Tree Regressor, Random Forest Regressor, VotingRegressor, BaggingRegressor, AdaBoost Regressor, GradientBoostingRegressor, and XGBoost. XGBoost turned out to be the best model with accuracy= 96.04.


### Best parametes

``` python
{'Model_fit__n_estimators': 200,
  'Model_fit__max_depth': 5 }
```

### Feature importances

<img src = "https://github.com/ahmedsaeed620/Price-prediction-of-used-cars/blob/main/images/ss.png" width = 850 height = 400/>

## Technologies Used

[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)](https://www.python.org)
[![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org) 
[![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com) 
[![](https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white)](https://www.anaconda.com)


Link My accaount in Kaggle : [Ahmed elsaied](https://www.kaggle.com/ahmedsaied3122)

Link My notebook in Kaggle : [Price prediction of used cars](https://www.kaggle.com/code/ahmedsaied3122/cars-price-prediction-with-accuracy-96-04)







