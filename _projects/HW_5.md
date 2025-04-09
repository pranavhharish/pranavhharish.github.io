---
name: HW_5
tools: [altair, bigfoot, data-visualization]
image: assets/post1.html
description: This is a "HW_5"!
custom_js:  
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# 📊 Bigfoot Sightings Visualizations

## 🌍 Interactive Map

This map visualizes reported Bigfoot sightings across the United States, plotted using geographic coordinates. The U.S. state boundaries are rendered from a TopoJSON layer, and each sighting is marked as a point. I encoded longitude and latitude as positional encodings and used color to represent different states, making it easier to distinguish spatial clusters. Tooltips provide additional context like location and date of the report. I cleaned the dataset by dropping rows with missing latitude, longitude, or state values. The projection used is albersUsa to fit the continental U.S. properly. This map offers an intuitive geographic overview and uses simple visual encodings to convey meaningful insights.

<iframe src="/assets/plot2.html" width="720" height="500" style="border:none;"></iframe>

---
## 🔁 Interactivity Discussion

The interactive component is present in the map. Users can click to reveal detailed tooltips for each sighting, and state-based color coding helps users compare regions quickly. This interactivity improves engagement and aids deeper geographic exploration without visual clutter.

---
## 📈 Sightings by Decade

This bar chart shows the number of Bigfoot sightings aggregated by decade. To simplify the crowded year-by-year data, I transformed the raw date field into years and then grouped it into decades. The x-axis encodes decades as ordinal data, and the y-axis shows sighting counts as quantitative data. Color was not necessary in this plot for clarity. This visualization helps reveal broader trends over time, such as peaks or declines in reports. Compared to Homework #5, I modified the x-axis granularity and used Altair for consistency with the current assignment.

<iframe src="/assets/plot1.html" width="720" height="450" style="border:none;"></iframe>

---


## 🔗 Resources  
[📁 The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv)  
[📓 The Notebook](https://github.com/pranavhharish/pranavhharish.github.io/blob/main/python_notebooks/test_generate_plots.ipynb)