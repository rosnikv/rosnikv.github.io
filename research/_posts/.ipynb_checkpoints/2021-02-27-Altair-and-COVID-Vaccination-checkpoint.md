---
layout: post
category: research
title: 'Altair and Covid Vaccination Data'
date: 2020-11-28 20:55
mathjax: true
---

## A note on python library 'Altair' and Vaccination data

A data scientist or data analyst demonstrating storytelling using interactive plots with data is unavoidable in the pipeline. Recently, I came across the python library called ["Altair"](https://altair-viz.github.io/getting_started/overview.html). 

> Altair provides a Python API for building statistical visualizations in a declarative manner. By statistical visualization we mean: ..

The Altair website explains it well and well-documented with many examples and case studies of interactive visualisations. You can see below one of the cool plots created with a few lines of python code:

```python
import altair as alt
from vega_datasets import data

source = data.unemployment_across_industries.url

selection = alt.selection_multi(fields=['series'], bind='legend')

alt.Chart(source).mark_area().encode(
    alt.X('yearmonth(date):T', axis=alt.Axis(domain=False, format='%Y', tickSize=0)),
    alt.Y('sum(count):Q', stack='center', axis=None),
    alt.Color('series:N', scale=alt.Scale(scheme='category20b')),
    opacity=alt.condition(selection, alt.value(1), alt.value(0.2))
).add_selection(
    selection
)
```

Upon selecting the options in `legend`, you would be able to see that particular option highlighted in the plot. I hope these small interactions contribute a lot to understanding and interpreting the data via visualizations.

{% include example_plot.html %}


During this pandemic time, one who does data analysis played a vital role in consolidating data related to corona across the globe and made it interpretable for a layman with the help of small but relevant interactions. One of the examples is [corona-data](https://corona-data.ch/) website which has the Switzerland COVID info.

Recently, Kaggle has published the `COVID-19 World Vaccination Progress, Daily and Total Vaccination for COVID-19 in the World` data set. This data set is useful to answer questions such as:
> 1. Which country is using what vaccine?
> 2. In which country the vaccination programme is more advanced?
> 3. Where are vaccinated more people per day? But in terms of percent from entire population ?

To demonstrate, I have used the vaccination data and tried to plot what per cent from each country's population are vaccinated and what vaccines are used by each country. You can see the plot below (`mouseover`: tooltip will help you provide more details on the data point!)

{% include chart.html %}

It is super easy to integrate the Altair generated plots into your own website. Altair library allows you to save your plots into an HTML file  (also, other different image formats and JSON file). For example, all you have to do in a Jekyll-now static website generator is include the generated HTML in the `_includes` directory and use the __liquid template language__ within your markdown file;

```python
{% include chart.html %}
```

P.S: I have done the same with this post  :metal: :octocat:



