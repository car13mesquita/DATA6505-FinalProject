# Citi Bike Analysis
![Citi Bike Logo](images/citibike_logo.png)

## Introduction
Citi Bike is a popular bike-sharing service in New York City, Hoboken, and Jersey City that allows users the flexibility of having a bike at their disposal whenever they need it without the hassle of bike storage and maintenance. The service offers memberships for frequent users and also has pricing for those one-time users visiting the area to ride around and explore.

Given that bike and scooter shares are becoming more common, especially in urban areas, we wanted to analyze the who, when, where, and how of the Citi Bike service to see if it was being used more for business purposes like commuting or more by leisurely users looking to have some fun.

## Data Source
The dataset used was the official Citi Bike data available at https://ride.CitiBikenyc.com/system-data. The dataset provides insight into the usage of Citi Bike in the Hoboken and Jersey City area for a period of 12 months from December 2021 to November 2022.

| Feature Name | Definition | Key | Data Type |
|--------------|------------|-----| --------- |
| ride_id | _Unique ID for ride identification_ | ... | object |
| rideable_type | _Type of bike_ | __classic_bike = Tradational Bike, electric_bike = E-Bike, docked_bike =unknown__ | object |
| started_at | _Day and time ride started_ | ... | object |
| ended_at | _Day and time ride ended_ | ... | object |
| start_station_name | _Name of the starting station_ | ... | object |
| start_station_id | _Unique ID of the starting station_ | ... | object |
| end_station_name | _Name of the ending station_ | ... | object |
| end_station_id | _Unique ID of the ending station_ | ... | object |
| start_lat | _Latitude of the starting station_ | ... | float64 |
| start_lng | _Longitude of the starting station_ | ... | float64 |
| end_lat | _Latitude of the ending station_ | ... | float64 |
| end_lng | _Longitude of the ending station_ | ... | float64 |
| member_casual | _Membership type of the rider_ | __member = Membership, casual = No membership__ | object |

## Conclusion
Based on our analysis, it appears that Citi Bikes are typically used for business more than pleasure.
* The busiest bike stations are ones near train stations which will allow commuters access to New York City or other parts of New Jersey.
* Usage is most popular during the morning and evening rush hour, but especially the evening. There are also more users in the summer when the weather is typically warmer and it is more pleasant to be outside.
* Riders are using Citi Bikes more during the week than on the weekend, and there are more members using the service than non members.

While this suggests more users are using Citi Bikes for business, About one-third of Citi Bike usage does appear to be for leisurely purposes. It may be the case that this usage helps Citi Bike on weekends in the spring and summer, but the true heroes are the commuters braving the elements to continue to patron Citi Bike in the colder winter months.

Click [here](https://github.com/car13mesquita/DATA6505-FinalProject/blob/main/analysis.ipynb) for the full analysis.

Click [here](https://github.com/car13mesquita/DATA6505-FinalProject/blob/main/summary.ipynb) for the detailed summary.

## Question for Further Analysis
* Can a user be advised on whether or not they as an individual should become a member? This would require additional fields in the data such as a member ID so rides could be connected to unique users.
* What impact does traffic have on ride duration at different times? Additional information on speed and routes traveled would be needed as well as traffic data for the time periods analyzed.
* Do more residents use the service or tourists to the area? In order to analyze this, Citi Bike would need to capture address information of their users. This may be included in payment information Citi Bike collects, but it was not available in the data set.
