# Visualization of Life Expectancy and GDP Variation Over Time - PowerBi

## Description of the Project
In this project, you will employ some of the Power BI skills you have learned to construct a series of related reports and a dashboard from a single data source.

You will be using visualizations that include scatter charts and bar charts to create reports that will provide insight about our semantic model, including Life Expectancy by Year and GDP Per Capita by Year.

You will practice every phase of a full life-cycle report and dashboard development, including loading data, cleaning data, correcting errors, and choosing and configuring vizualizations.

## Description of the semantic model
The Gapminder dataset SampleDataWS combines data from multiple sources into coherent time-series information about life expectancy over time for countries and regions around the world.

### Instructions
1. Load the data set.

##  Fix Data Import Issues
When we loaded the data, many errors occurred. This is normal. Data is never in perfect shape for analysis when we get it — we need to clean it first. Let's start our cleaning and transforming journey by troubleshooting the issues.
The errors we received are mainly due to several cells containing NA in the life_exp column. To resolve this issue, we have to change the life_exp data type to Decimal Number and then convert the error values to null.

There are also some errors in the year column. To resolve this issue, we have to replace errors with the value 1919.

## Clean, Transform, and Load the Data
Let's continue cleaning and transforming our data to get it ready for analysis and visualization.

Here are some cleaning and transformation tasks we want to complete:

The Name column actually contains country names and should be renamed to Country.
The name life_exp isn't meaningful. Rename it as Life Expectancy.
We won't use the g77 column for our analysis. Let's remove it.

## Relationship Between Years and Life Expectancies
At this point, our semantic model is ready for analysis and visualization. We'll look at how life expectancy evolves by year and by region.

We will plot a scatter chart between Year and Life Expectancy. The expected result is the following.

### Instructions
1. Create a scatter chart with the Year column as the x-axis and Life Expectancy as the y-axis.

2. Add the Region column to the Legend to color the data-points based on the regions.

3. We can resize the data-points using the Population by dragging Population to Size.

##  GDP Per Capita Variation Over Time
From the scatter chart on the previous screen, we can see that life expectancy grows over time. Let's see if the GDP per capita variation over time follows the same trend. We'll use the Stacked Column Chart to do so.

### Instructions
1. Reproduce the expected result by doing the following:
  Select the Stacked Column Chart from the Visualization panel.
  Add Year, GDP percap, and Region respectively to Axis, Value, and Legend.

## Design a Dashboard
ow that we have two visuals, it's time to create a page to put it all together.

This dashboard will contain the two visuals and a slicer. We'll also allow interactions.

The slicer is on the regions. We'll edit interactions for the stacked column and scatter charts.

The expected effect is that when we select Asia on the gdp_percap by year and region stacked column chart, the Avg of life_exp by region and year scatter chart doesn't filter to only the Asian region as the other charts do.
