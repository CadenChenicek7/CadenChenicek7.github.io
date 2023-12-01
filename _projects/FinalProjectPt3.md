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


# Final Project Pt. 3

## Plot 1:

<vegachart schema-url="{{ site.baseurl }}/assets/json/floors_per_year.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/count.json" style="width: 100%"></vegachart>

## Write up:

For this plot I decided to use the building inventory dataset. This graph is a visualization of buildings built from the 1800's until present, and how many floors they have. I was hoping to get a more positive trend as I expected more floors as the years went on, however it seemed to stay fairly stagnant at 10 floors around the 1920s. I first cleaned the data by filtering out all of the incorrect dates or rows that were missing a date, then I looked at the data frame and checked if there was any features I could use to further classify these points. I went with usage description as I found that to be the most categorical feature. This was an entirely new plot from my HW #7. For this visualization I attempted to get some form of interactivity other than the provided, however I couldn't figure out how to do the link two plots as was shown in the doccumentation of altair. What I was trying to accomplish with interactivity was an option to select an area of the graph and the count of each usage description on a histogram below the scatter. Unfortunatly I could not get that working in time.

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
