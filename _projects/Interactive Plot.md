---
name: Vega Lite Homework 6  Interactive Plot Project
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

This visualization presents an interactive box plot that highlights the distribution of license numbers across different license types. The box plot structure makes it easier to identify the variability, median values, and potential outliers for each license type.

Design Choices
1.Encoding: The x-axis encodes the categorical variable License Type, displaying each type as a distinct category. The y-axis encodes the numeric variable License Number, showing the range and distribution for each license type. 2.Color Scheme: A conditional color scheme is applied to the box plot. The selected license type is highlighted in its unique color, while unselected types appear in a light gray. This enhances the user’s ability to focus on a specific category while still retaining context for all categories. 3.Tooltips: Tooltips display the specific license type and associated license numbers, offering detailed insight into individual data points.

Interactivity: A dropdown filter allows the user to dynamically select a license type. The corresponding box plot is highlighted, making it easier to analyze individual distributions. Zoom and pan interactions are enabled to allow users to focus on specific regions of the plot. This is particularly useful for datasets with high variability or a large number of license types.

Data Transformations The raw dataset underwent several transformations: Non-numeric values in the License Number column were coerced to NaN and subsequently dropped to ensure clean and accurate plotting. The cleaned license numbers were converted to integers for consistency. A unique list of license types was extracted to populate the dropdown filter. These transformations ensured that the data was properly structured and free of errors, making it suitable for Altair's visualization methods.

## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/e81209bf6de87a20f179f1d815c9c0cd3410adf3/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/f0453dd6d933d56912be07bfaabdaa01d99c660b/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/e81209bf6de87a20f179f1d815c9c0cd3410adf3/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/ssdd8/ssdd8.github.io/blob/f0453dd6d933d56912be07bfaabdaa01d99c660b/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

