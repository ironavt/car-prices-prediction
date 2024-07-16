# Car prices prediction
## Project description

Our customer is a used car sales service that developes an application in order to attract new clients. This app helps to determine a market price of user's car.

Following criteria are essential for the customer:
* prediction quality
* time required for model trainig
* time required for prediction

## Dataset description

Dataset objects are entries crawled from car profile forms:
* `DateCrawled` — date the form was downloaded on from a database
* `VehicleType` — car body type
* `RegistrationYear` — year of car registration
* `Gearbox` — gearbox type
* `Power` — horsepower (hp)
* `Model` — car model
* `Kilometer` — car mileage (km)
* `RegistrationMonth` — month of car registration
* `FuelType` — fuel type
* `Brand` — car brand
* `Repaired` — was the car in repair or not
* `DateCreated` — car profile creation date
* `NumberOfPictures` — number of car photos
* `PostalCode` — postal code of a user who owns a car profile
* `LastSeen` — last user activity date

Target feature:
* `Price` — price (euro)

# Conclusion
* Dataset has a lot of outliers and missing values.
* * I marked outliers as **NaN** values and removed only objects with 3 or more missing values.
* * For objects left I changed **NaN**s to **unknown** values in categorical features.
* All models except dummies showed RMSE score that meets reqirements.
* Random Forest Regressor showed itself to be the slowest one.
* Linear Regression was the fastest to fit and to predict. It has the worst RMSE score but it still fits requirements.
* CatBoost fits much slower than LGBM but makes predictions faster.
* LGBM fit time is the second after Linear Regression

LightGBM model was chosen with **RMSE** score of **1429**