# Car_Sales_Dashboard

# Car Sales Report

## Overview
This report presents an in-depth analysis of a car dataset containing various attributes related to different car models, manufactures and dealership.
The objective of this report is to explore the dataset, derive meaningful insights and develop predictive models to estimate key outcomes such as:
+ Top selling models
+ Dealer performance
+ Monthly trends
### Tools Used
+ Excel for data cleaning
+ Pivot table
+ SQL for data manipulation
+ Power Bi for visualization
### Sql Queries
How many Category of color
``` SQL
select color, count(distinct color) as number_of_color_category
from
new_car_datasets
group by color;
```
Retrieve the total number per body type
``` SQL
select body_style,
count(*) as total_number_per_body
from new_car_datasets
group by body_style;
```
Retrieve total number per transmission type
``` SQL
select transmission, count(*)
from new_car_datasets
group by transmission;
```
Retrieve total sales amount for the year 2022
``` SQL
select sum(Price) as 2022_total_sale
from new_car_datasets
where year(Date) = 2022;
```
Retrieve sale for 2022 and 2023
``` SQL
select sum(Price)
from new_car_datasets
where year(Date) in (2022, 2023);
```
Retrieve average selling price
``` SQL
select avg(Price)
from new_car_datasets;
```
Retrieve average selling price for 2022 and 2023
``` SQL
select avg(Price)
from new_car_datasets
where year(Date) in (2022, 2023);
```
### Power Bi Visualization
