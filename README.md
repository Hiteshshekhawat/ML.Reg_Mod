# SEOUL BIKE SHARING DEMAND PREDICTION
> REGRESSION 

## PROBLEM DESCRIPTION

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern.

The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes
## DATA DESCRIPTION

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

Attribute Information:

Date : year-month-day

Rented Bike count - Count of bikes rented at each hour

Hour - Hour of he day

Temperature-Temperature in Celsius

Humidity - %

Windspeed - m/s

Visibility - 10m

Dew point temperature - Celsius

Solar radiation - MJ/m2

Rainfall - mm

Snowfall - cm

Seasons - Winter, Spring, Summer, Autumn

Holiday - Holiday/No holiday

Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
## Main Library To Use

* Pandas for data manipulation, aggregation.

* Matplotlib and seaborn for visualisation and behaviour with respect to the target variable.

* Numpy for computationally efficient operations.

* Scikit learn for model training, model optimization and metrics calculation.
## LINKS 

COLAB LINK: 

https://colab.research.google.com/drive/1m2J8uo3H0bdhKXBCHOnmenu_pS2do8AP?usp=sharing

DATASET LINK:

https://drive.google.com/file/d/1dZ7p614gC_iwxHwcj-1N0Lc155AGMTJS/view?usp=sharing

> DATASET - ALMABETTER




## CHALLENGES  FACED:

* Removing Outliers.

* Encoding the categorical columns.

* Removing Multicollinearity from the dataset.

* Choosing Model explainability technique.
## SUMMARY AND OBSERVATION

* The maximum bikes were rented in summer i.e.3500 followed by autumn and spring whereas the minimum bikes were rented in winter which is around 900

* The total functioning day were 8467 i.e. 96.6% and holidays were around 295 i.e. 3.4%.

* Summer has the highest number of bikes rented, 37%. This could be because of the vacation mood created in summer and also the increase in the number of tourists. Winter however is the season where the least number of bikes are rented, 8%.

* Maximum number of booking is done on Sunday and Tuesday whereas minimum number of booking is done on monday.

* Maximum Bike were rented between 10(°C) to 30(°C) from this we can clearly say that people generally book the bike when temperature is normal.

* Most number of bikes are rented when there is no snowfall or rainfall.

* Majority of the bikes are rented for a humidity percentage range of 20 to 80.

* The highest number of bike rentals have been done in the 18th hour, i.e 6pm, and lowest in the 4th hour, i.e 4am.

* The most of the booking are in working over. We can say that people use them from home to office and office to home.
## ML OBSERVATION

Random Forest Regression is the best performing model with an r2 score of 0.65.

All 3 models have been explained with the help of SHAP library.

Both linear and ridge regression both have r2 score of 0.45.

Temperature and Hour are the two most important factors according to all the models.
