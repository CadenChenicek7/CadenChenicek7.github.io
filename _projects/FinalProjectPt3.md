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


# Video Game Sales and Ratings 1985-2016

## Plot 1:

<vegachart schema-url="{{ site.baseurl }}/assets/json/video_games.json" style="width: 100%"></vegachart>

## Data Summary:



## Contextual Data:

<img src="{{ site.baseurl }}/assets/pngs/gameRevenue.png" alt="context1" />

[Game Revenue Source](https://www.visualcapitalist.com/50-years-gaming-history-revenue-stream/)

<img src="{{ site.baseurl }}/assets/pngs/regionalSales.png" alt="context1" />

[Regional Sales Source](https://www.stat.cmu.edu/capstoneresearch/spring2020/315files/team20.html)

## Search The Data & Methods

Below is where we I put links to both the data and the analysis code as buttons:

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/CadenChenicek7/CadenChenicek7.github.io/blob/main/python_notebooks/data/Video_Games.csv" text="Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CadenChenicek7/CadenChenicek7.github.io/blob/main/python_notebooks/FinalProjectPt3.ipynb" text="The Analysis" %}
</div>
