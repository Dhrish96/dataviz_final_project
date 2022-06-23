# Data Visualization 

> Author : Dhrishya Menon 

## Mini-Project 2 Report


**"The Dataset that has been used for the Interactive plot and Linear Regression plot is that of the U.S. births data for the years 2000 to 2014"**

*The link for the Dataset chose for the first and third plot is:
[U.S. Birth Data](https://raw.githubusercontent.com/reisanar/datasets/master/us_births_00_14.csv)*


**"The Shapefile that has been used for the Spatial Visualization is that of Florida lakes"**

*The link for the Shapefiles can be obtained from:
[Florida Lakes Shapefile](https://raw.githubusercontent.com/reisanar/datasets/master/Florida_Lakes.zip)*

***
#### The packages and libraries installed in the project and loaded are:

1. Tidyverse
2. ggplot
3. plotly
4. dplyr
5. RColorBrewer
6. htmlwidgets
7. sf
8. broom

***
> The main questions that have been asked are as follows:

* What were the original charts you planned to create for this assignments? What steps were necessary for cleaning and preparing the data?

* What story could you tell with your plots? What difficulties did you encounter while creating the visualizations? What additional approaches do you think can be use to explore the data you selected?

* How did you apply the principles of data visualizations and design for this assignment?


### Interactive Plot

**Displaying the change in the total number of births throughout the years**

The original dataset is grouped by with the help of the group_by() function and the number of births are summed up a new sub-dataset is created.

The library of plotly is used to create an interactive graph which is much more visually appealing. The original graph that was intended to be plotted was a barplot which displayed the total births that occurred in each month, and the changes occurring across the years would be displayed by clicking the play button. 

The plot basically enables the user to observe the total no. of births that have occurred in each month throughout the years 2000 to 2014. 

The code for multiple trace animation is used and a scatter plot is plotted which is displayed with the help of "markers+lines" which makes it easier to get the births that have been recorded in a particular month. The layout function helps in labelling the axes and title of the plot and lastly, the animation slider is modified to display the "Year".

The interactive plot is then saved as a standalone **HTML File** which can be accessed via:

[Birth Data](https://raw.githubusercontent.com/Dhrish96/dataviz_final_project/main/project-02/birth_data_figure.html)

***

### Spatial Visualization

**Displaying the largest lake according to area in Florida County**


In the initial step the shapefile of the data being used is loaded. The shapefile format is a geospatial vector data format for geographic information system (GIS) software.

The str() function is used to show the internal structure of dataset. The dataset is then sorted in descending order to help obtain the largest lake in terms of area in the Florida county. geom_sf() is used to display spatial information.
Initially, the graph is re-projected to a Mollweide CRS using coord_sf(crs = "+proj=moll +ellps=WGS84"), this made the plot to become a bit more difficult to read. 

![Graph for Largest Lake](https://github.com/Dhrish96/dataviz_final_project/blob/main/figures/Areawise_lake.png)

***

### Linear Regression Model 


The dataset is grouped according to year and the number of births is summed up and stored in a new sub dataset which is used to plot the linear regression graph. The "broom" library is used to tidy up the dataset and the linear regression is viewed with the help of summary() and glance() functions. 


![Graph for Largest Lake](https://github.com/Dhrish96/dataviz_final_project/blob/main/figures/linear_regression.png)

***
