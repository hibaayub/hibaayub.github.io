---
name: Homework 6
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: These are my visualizations for homework 6.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Visualization 1

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>

This histogram visualizes the distribution of buildings based on their "Year Constructed." 
The x-axis represents the binned "Year Constructed," divided into 20 bins to provide a clear distribution 
overview. The y-axis shows the count of buildings in each year bin, and I included a tooltip to display 
the year and count when hovering over the bars. The design choice of binning allows for an easier
interpretation of trends over time. I did not perform any transformations on the data, as the raw year 
data was sufficient for the analysis. The interactivity of this visualization enables users to zoom in or 
out, allowing for a more detailed exploration of specific time periods.


## Visualizations 2

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>

The scatterplot visualizes the relationship between "Square Footage" and "Total Floors" of buildings, 
with each point representing an individual building. The x-axis shows the square footage, while the 
y-axis represents the total number of floors. The scatterplot effectively illustrates whether 
newer or older buildings tend to be larger or have more floors. No data transformations were necessary 
for this plot, as the raw values were directly used. The interactivity on this plot also allows users 
to zoom and pan and explore specific areas of the dataset more easily.

<!-- these are written in a combo of html and liquid --> 

Below are the links to the data and the analysis.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/hibaayub/hibaayub.github.io/blob/main/Workbook.ipynb" text="The Analysis" %}
</div>

