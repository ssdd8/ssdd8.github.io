---
name: Vega Lite Homework 6 Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/plot2.png
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
<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/plot2.json" style="width: 100%"></vegachart>

The second plot is an interactive scatter plot that visualizes the relationship between the original license numbers and their binned equivalents while highlighting license types. This chart allows users to explore how licenses are distributed across various types and observe clusters or outliers in the data.

Design choices include using color to encode the License Type, allowing users to differentiate among them visually. A dropdown filter was implemented to let users select a specific license type, making it easier to focus on a subset of the data. Additionally, I added a brush selection tool to enable users to highlight regions of interest directly within the plot. The x-axis represents the binned license numbers (to reduce granularity), while the y-axis shows the original license numbers. Tooltips provide additional context by displaying exact license numbers and types when hovering over a point.

Data transformations included cleaning the License Number column by coercing invalid values to NaN, dropping rows with missing data, and converting the column to integers. A binned version of the license number was created for systematic grouping, and a unique list of license types was extracted for the dropdown filter.

Interactivity enhances this visualization by allowing users to dynamically explore the dataset. The dropdown filter narrows the view to specific license types, while the brush selection highlights data points in a chosen region. This makes the scatter plot not only visually appealing but also an effective exploratory tool.
​

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

