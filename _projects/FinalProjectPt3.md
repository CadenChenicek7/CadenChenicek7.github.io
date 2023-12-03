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
#### Work done by Caden Chenicek

## Visualization:

<vegachart schema-url="{{ site.baseurl }}/assets/json/video_games.json" style="width: 100%"></vegachart>

## Data Summary:

This Dataset is a collection of all video games from 1985-2016 and contains information such as sales, ESRB rating, critic rating, regional and global sales, the platform, and the developer. Using this data, I created the visualization that can be seen above. This is all video games plotted based on their weighted critic score and their global sales in millions. The x-axis is the video games sales and the y-axis is the calculated score they recieved. The algorithm used to calculate the weighted critic scores takes the user/player rating and the critic rating, then based on the number of users/critics it gives a weighted score per game. 

The visual is color coated by which genre each game falls under. This can be seen in the legend on the right. Hovering over a point will tell you the name of the game, the year it was released, and which console/platform the game was released for. You may see duplicate games, this is because many games where released for seperate platforms and their revenue per platform is accounted for individualy. Below the chart is a dropdown menu that allows for you to select a game developer. Doing so will highlight all of the games made by this developer and greyscale all of the games that are not. Feel free to zoom into the chart and explore the games with more detail, as it is sometimes difficult to pick out a game from the bunch. Both the X and Y axis will adjust according to your zoom.

Below are two pieces visualizations made by other authors that can be helpful in understanding more about the data that is charted above. The first visualization shows the video game industry's revenue as a whole and goes as recent as 2020. I think it is helpful to understand how large of an industry this really is along with understanding what platforms are bringing in the most money. If this chart was more recently done I think there would be a large spike in VR and cloud gaming revenue. The second visualization was done by students at Carnegie Mellon University, and shows the video game sales data per each region. Looking at the legend on the right you can see that North America is highly dominant in this field.

## Contextual Data:

<img src="{{ site.baseurl }}/assets/pngs/gameRevenue.png" alt="context1" />

[Game Revenue Source](https://www.visualcapitalist.com/50-years-gaming-history-revenue-stream/)

<img src="{{ site.baseurl }}/assets/pngs/regionalSales.png" alt="context1" />

[Regional Sales Source](https://www.stat.cmu.edu/capstoneresearch/spring2020/315files/team20.html)

## Search The Data & Methods

Below is where we I put links to the dataset and the analysis code as buttons:

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/CadenChenicek7/CadenChenicek7.github.io/blob/main/python_notebooks/data/Video_Games.csv" text="Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/CadenChenicek7/CadenChenicek7.github.io/blob/main/python_notebooks/FinalProjectPt3.ipynb" text="The Analysis" %}
</div>
