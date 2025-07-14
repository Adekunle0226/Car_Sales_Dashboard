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

### Power Bi Visualization
