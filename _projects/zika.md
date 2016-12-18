---
layout: project
title: Zika Story
date: 2016-08-10
thumbnail: zika_th.jpg
thumb_alt: Map of Recife, Brazil.
include: zika
view_site: http://apps.frontline.org/zika-water/
roles: 
 - user experience
 - visual design
 - illustration
 - HTML/CSS
---

[Zika Uncontained](http://apps.frontline.org/zika-water/) is a long form text article with integrated video and graphics. Its goal is to show how infrastructure problems in Brazil have worsened the spread of Zika. The project was spearheaded by reporter [Katie Worth](https://twitter.com/katieworth) and video producer [Michelle Mizner](https://twitter.com/michellemizner), I worked with them to nail down the user experience and execute the visual design.

## The Illustrations
Each chapter is marked with an illustration of the mosquito life cycle. The tone of the illustrations had to match the seriousness of the piece. I decided on realistic mosquito illustrations rendered in hand-drawn pencil lines.

{% include inline-col.html inline_img='zika_mosq.jpg' class='topbtm-border' alt='Mosquito life cycle illustrations' %}

I tried a couple of different directions before arriving at this solution. In an earlier iteration I looked at more abstract, iconic patterns inspired by Recife, Brazil, the city that is the focus of the article. But these proved to feel too playful and didn’t match the seriousness of the story.

{% include inline-col.html inline_img='zika_ill_alt.png' class='topbtm-border' alt='Recife, Brazil chapter illustrations' %}

## The Map
The article focused on one neighborhood in Recife, Brazil where the mosquito problem was at its worst. We wanted to show a map of the city and highlight the neighborhood to orient the user. It was important to show the relationship of this one small neighborhood to the larger city.

{% include inline-wide-thirds-unequal.html mod='unequal' inline_img1='zika_map_lg.jpg' inline_img2='zika_map_med.jpg' inline_img3='zika_map_sm.jpg' alt1='Map of Recife, Brazil, desktop view.' alt2='Map of Recife, Brazil, tablet view.' alt3='Map of Recife, Brazil, mobile view.' %}

The key infrastructure problem in the story is water access. And the map illustrates the irony of a city surrounded by ocean and rivers, but a city that struggles to deliver constant running water to its residents—particularly its poor. The information card introduces data that is covered in greater detail later. I treated the map and info card as self-contained, responsive layouts with unique breakpoints and type size optimization.

## The Charts
Our reporter collected powerful data about water, income and mosquitos for the city of Recife. This was the early driver behind the story. We needed visuals that could communicate a connection between income, water access and a higher mosquito population. After many iterations we chose a direction that focused on the ten wealthiest and ten poorest neighborhoods. The water graphics are very stripped down, they show how many neighborhoods have constant running water and how many do not. The mosquito graphics illustrate that the poorer neighborhoods have higher mosquito populations.

{% include inline-col-stack.html inline_img1='zika_water_chart.jpg' inline_img2='zika_mosq_chart.jpg' class='topbtm-border' alt1='A chart showing the correlation between wealth and water access in Recife, Brazil.' alt2='A chart showing the correlation between wealth and mosquito index in Recife, Brazil.' %}

I looked at many directions for visualizing this data. Our final solutions were the clearest and most compelling, and they represented the data in the most fair and accurate way. Here are some earlier design options for the mosquito and water graphics.

{% include inline-col.html inline_img='zika_chart_sketches.png' class='topbtm-border' alt='Sketches of charts and graphs showing income, water access and mosquito index data for Recife, Brazil.' %}

