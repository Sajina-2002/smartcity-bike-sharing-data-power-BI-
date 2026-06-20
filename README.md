# smartcity-bike-sharing-data
## (Power-BI)


## Table of Contents
- [1.Project Overview](-Project-Overview-)
- [2.Data source](-Data-Source-)
- [3.Tools & Technologies](-Tools-&-Technologies-)
- [4.Data Cleaning & Preparation](-Data-Cleaning-&-Preparation-)
- [5.Formulas and functions/DAX](-Formulas-and-Functions-)
- [6.Exploratory Data Analysis (EDA)](-Exploratory-Data-Analysis-)
- [7.Key Insights](-Key-Insights-)
- [8.Recommendations](-Recommendations-)
- [9.Conclusion](-Conclusion-)

## Project Overview:
Public bike-sharing systems generate continuous data from hundreds of stations across different cities. The task is to analyze this real-time bike station dataset to understand station performance, usage efficiency, and operational patterns across cities.
Applying Power BI skills—from data cleaning and modeling to DAX and dashboarding—to turn raw data into actionable urban mobility insights.

## Data Source:
Real time data source from Entri Elevate Academy.

## Tools & Technologies:
Language: DAX(Data analysis expressions) and (Power Query Formula Language)
Database: SQL 
Visualization: Power BI
Documentation: microsoft word

## Data Cleaning & Preparation:
Data’s got transformed and cleaned in power queory and fact and dimension tables are created.

### Fact table:
•	Number 
•	Bike stands 
•	Available Bike stands 
•	Last update
### Dim_City
•	Contract name
•	Number
### Dim_Station
•	Number
•	Latitude 
•	Londitude
•	(position are split into two different columns latitude and longitude)
### Dim_Status
•	Number 
•	Status 
•	Banking
•	Bonus

## Formulas & Functions / DAX:
•	Total Available Bikes = SUM('Fact Table'[Available Bikes])
•	Total Capacity = SUM('Fact Table'[Bike Stands])
•	Total Station = COUNT('Fact Table'[Number])
•	Utilization% = DIVIDE([Total Available Bikes],[Total Capacity]) *100
•	Empty Stands = SUM('Fact Table'[Available Bike Stands])

## Exploratory Data Analysis (EDA):
The model follows a star schema approach, where:
Fact table is at the center
Dimension tables surround it
•	Simplifies data analysis
•	Improves query performance
•	Supports scalable reporting
The data model is designed using best practices with a fact and dimension structure, enabling efficient data processing, accurate reporting, and meaningful insights.
It forms the foundation for building interactive dashboards and performing advanced analytics in Power BI.

<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/77677307-a1fe-4f34-9e95-58f6ad21dd4e" />
<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/d9d7b14e-6c2a-43ae-8bcd-0ea273642054" />
<img width="300" height="200" alt="image" src="https://github.com/user-attachments/assets/bebea603-e7fa-4b11-9394-336e09bea8c6" />
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/ab1b8b07-231a-46ff-acbe-8fcdacb8a0d4" />

## Key Insights:
•	High-capacity areas are not always efficiently utilized.
•	Indicates operational inefficiencies or uneven demand patterns.
•	Closed stations may reduce service coverage.
•	High-capacity regions should be prioritized for maintenance and monitoring.
•	Growth trend is positive, but distribution still needs optimization.
•	Geographic insights support better station placement and rebalancing.

## Recommendations:
•	Bike system has high capacity but low utilization
•	More than half of stands are empty, indicating imbalance
•	Certain locations/contracts are overperforming, others underperforming
•	Operational focus needed on:
	Bike redistribution
	Demand forecasting
	Station optimization

## Conclusion:
This report highlights that while the bike-sharing system has strong infrastructure and wide coverage, it suffers from low utilization and inefficient distribution.
By improving data-driven decision-making, the system can:
•	Increase efficiency
•	Enhance user satisfaction
•	Maximize return on investment








