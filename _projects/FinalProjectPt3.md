---
name: Video Game Sales Throughout History
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: By Caden Chenicek
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Video

## Plot 1:

<vegachart schema-url="{{ site.baseurl }}/python_notebooks/video_games.json" style="width: 100%"></vegachart>

## Write up:



## Plot 2:

<vegachart schema-url="{{ site.baseurl }}/assets/json/pie_chart.json" style="width: 100%"></vegachart>

## Write up:

For my second plot I went with a much more simple visual approach and focused on transforming the data to fit the visualization. I used the licences data set for this visual and wanted to know the count of each type of licence that was administered. I first had to do some experimenting with different pandas functions to determine the best way to get a data frame of unique value counts and found that there is a fairly simple solution thanks to pandas. After I had the desired data frame I then looked at the docs to determine how to make a pie chart. For the coloring I decided to use a unique color per each type of license. I was suprised with how many cosmetic licenses where administered, that being the second most common after detective board.

## Search The Data & Methods

Below is where we I put links to both the data and the analysis code as buttons:

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="Plot 1 Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CadenChenicek7/CadenChenicek7.github.io/blob/main/python_notebooks/HW10Chenicek.ipynb" text="The Analysis" %}
</div>

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="Plot 2 Data" %}
</div>
