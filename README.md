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