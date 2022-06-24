---
title: "Project_03_Report"
author: "Dhrishya Menon"
date: '2022-06-24'
output: html_document
---

## Mini-Project 3 Report

***
#### The libraries installed in the project and loaded are as follows:

1. Tidyverse
2. ggplot
3. viridis
4. dplyr
5. ggridges
6. forcats
7. viridisLite
8. lubridate
 
***

**"The Dataset used for the project is obtained from FSU for a station at Tampa International Airport (TPA) from 2016 to 2017"**

[Florida Climate Center](https://climatecenter.fsu.edu/climate-data-access-tools/downloadable-data)


*The link for the Dataset chosen for recreating the graphs:
[Tampa Weather Data](https://github.com/reisanar/datasets/raw/master/tpa_weather_16_17.csv)*



> The main task of Part 1 was to recreate six graphs which makes use of faceting and ridges:


#### Question (a)

The initial step is to convert the numeric columns of "month" into written characters, the function **as.factor** is made use of  whose main function is to return the original object of a class with the requested column specified as a factor rather than numeric.

To obtain the actual graph according to the image given, the function of **facet_wrap** is performed on the column month and the months are divided into different grids and the data is displayed in the form of a histogram. 

![Maximum Temp vs. Days](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\temp vs days_facet.png)


***

#### Question (b)

The second plot is the density plot which is evaluated using the kernel **epanechnikov** and the parameters of bw and lwd which set the bandwidth and line width respectively are also used to plot the graph.

![Density Plot](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\density_kernel.png)

***

#### Question (c)

The third plot is the density plot along with facet_wrap which is evaluated using the default kernel **gaussian** is used to plot the graph.The legend is omitted from being displayed by using the function *legend.position = "none"*

![Density Plot](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\density_and_facet.png)

***

#### Question (d) and (e)

Density ridges is plotted with quantile lines. By default, three lines are drawn, corresponding to the first, second, and third quartile. In the graph we plot only the second quartile is required. 

![Density Plot](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\Density_ridges.png)


***

#### Question (f)

Density ridges is plotted with quantile lines and the plot showcases the second quartile. The title of the legend is remo0ved and the labels appearing on the legend are also reversed in order 

![Density Plot Plasma](C:\\Users\\dhris\\OneDrive\\Desktop\\Notes\\Data Visualization\\Project_Screenshots\\Density_ridges_plasma.png)


***


