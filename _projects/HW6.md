---
name: Vega Lite Homework 6 Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization.png
description: This is a Homework 6 project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.json" style="width: 100%"></vegachart>

In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.


## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/935cf44cb30d505171ad31dcb494ceb70c893b33/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/935cf44cb30d505171ad31dcb494ceb70c893b33/Hw6.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/935cf44cb30d505171ad31dcb494ceb70c893b33/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/935cf44cb30d505171ad31dcb494ceb70c893b33/Hw6.ipynb" text="The Analysis" %}
</div>

