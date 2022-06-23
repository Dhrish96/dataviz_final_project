---
title: "Report for Data Visualization Mini-Project 1"
author: "Dhrishya Menon - dmenon2337@floridapoly.edu"
date: '2022-06-06'
output: html_document
---

**"The Dataset gives data from years 1984 to 2017 regarding the fuel economy produced during vehicle testing at the Environmental Protection Agency’s (EPA) National Vehicle and Fuel Emissions Laboratory"**

*The link for the chosen Dataset is:
[Fuel Data ](https://raw.githubusercontent.com/reisanar/datasets/master/fuel.csv)*

***

> All the relevant packages and libraries are installed and the required dataset was loaded into R studio. The columns were reviewed to get a better understanding of the steps needed and to make a visual assessment.

***

The Four Main Graphs which have been visualized are as follows:

* Graph for the Most Popular Class of Car
* Graph for the Most Popular Make of Car
* Graph for Most Fuel type used in the most popular make of car
* Graph for Annual Cost of Fuel used in the most popular make of car


I proceeded to select the columns that were relevant for creating graphs. The null values present were checked and subsequently dropped from the data set. It was identified that the column **transmission** contained 11 null values.

### First Data Visualization Graph

**Finding the Most Popular Class of Car**

![Graph for Most Popular Class of Car](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\popular_class.png)

The above graph is created using a new sub-data set derived from the original data set. The graph displays the number of different class of cars in the data set.
The main three class of cars that are popular in order are:
 1) Compact Cars
 2) Subcompact Cars
 3) Midsize Cars

Originally a scatter plot was tried but it was found to be too clustered and was not providing any meaningful information. 

***

### Second Data Visualization Graph

**Choosing the most popular make of car**

![Graph for Most Popular Car Make](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\car_make.png)

In the above graph, the three popular class of car are selected. The class of cars are then filtered to form a new second sub-dataset and a histogram of the Make of the car vs the total number of car in the respective make is displayed.
The most popular make of car is found to be **BMW**.

*RBrewColor Package* is used to display colors other than the default colors used in graphs.Theme function is made use of to display the text on x-axis to be more legible. 

Originally a pie chart was tried but as there are too many fields pie chart was not useful.

***

### Third Data Visualization Graph

**The most used type of fuel**

![Graph for Most Used Fuel Type](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\fuel_type.png)
In the above displayed graph, the most popular car make "BMW" is used to create a new data set having BMW sub-compact, compact and mid size car information.This is used to find out the type of fuel used. The classification of class of cars are distinguished with the help of colors.
In conclusion, it is found that **Premium type of Fuel** is the most used Fuel in BMW cars, followed by Regular fuel and Diesel and the number of Subcompact cars utilize more premium fuel.

*scale_fill_brewer* is used to assign the Spectral color palette to the graph.The x and y axis are appropriately labelled with the help og labs function.

Originally a bar graph without color palette was tried but adding class data provided more information.

***

### Fourth Data Visualization Graph

**The Annual Cost of Premium fuel**

![Graph for cost of premium fuel](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\premium_fuel.png)

The above graph displays the Boxplot of the Annual cost of premium fuel for BMW cars (sub-compact, compact, and mid size car). It is found that the Compact cars have lower annual median cost of fuel.

Originally a bar chart was tried but boxplot help show the difference in the cost for the fuels in a better fashion.

***

> 
**Conclusion** :
Based on the data, the most popular car for the past three decades (1984 to 2017) are sub-compact, compact, and mid size cars. More than 4,000 cars of this class are sold during this period. BMW is the most popular make among these cars. BMW sub-compact, compact, and mid size cars were found to mostly use premium fuel and lastly, annual cost of owning a compact car may be lower than sub-compact or mid-size car.

***



