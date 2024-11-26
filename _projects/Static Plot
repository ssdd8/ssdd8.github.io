---
name: Vega Lite Homework 6 Static Plot Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/plot1.png
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
<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot1.json" style="width: 100%"></vegachart>

The first plot visualizes the distribution of the number of licenses held by users. This distribution helps us understand the degree of engagement of users in terms of license acquisition. To create this, I grouped users by their first and last names, calculated the total number of licenses per user, and filtered out users who had only one license to focus on those with significant engagement.

In the design of the visualization, the x-axis represents the number of licenses (binned for clarity), while the y-axis represents the count of users falling into each bin. A bar chart was chosen for its simplicity and ability to communicate frequency distributions effectively. The steel blue color scheme was applied uniformly to highlight the data without introducing distracting visual elements. Data transformation included grouping and filtering steps to clean and simplify the dataset.

This plot is static because it does not allow user interaction. However, it provides a clear summary of the license count distribution, enabling stakeholders to spot trends or anomalies in user engagement.

## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/e81209bf6de87a20f179f1d815c9c0cd3410adf3/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/3ed1c323a4e8b2bcddc46fd595ec12bee81fd7fd/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/e81209bf6de87a20f179f1d815c9c0cd3410adf3/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/3ed1c323a4e8b2bcddc46fd595ec12bee81fd7fd/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
