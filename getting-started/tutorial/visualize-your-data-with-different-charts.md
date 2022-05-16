---
description: Visualizing Data with Different Charts
---

# Visualize Your Data with Different Charts

What kind of charts and graphs should you use to best show the data? This guide will help you pick the right visualization chart to suit all your needs.

Picking the right chart comes down to two questions: what does the data look like, and what are you trying to show?

In this article:

* Two Most Basic Kinds of Charts
  * Tables
  * Line Charts
* When You Only Have One Value
  * Number Visualization
* Comparing Metrics
  * Static Comparisons
  * One Measure Over Time
  * Multiple Measures Over Time
* Showing the Relationship Between Measures
* Breakouts
  * A metric with Several Groups
  * Categorical Breakouts Over Time
  * Relative Changes Among Categories Over Time

### Two Most Basic Kinds of Charts <a href="#_4bertauy5vdo" id="_4bertauy5vdo"></a>

Before we start, we should note: you don’t have to use every chart type to do proper analysis. Most of the time you’ll only need **tables** and **line charts**.

### Tables <a href="#_effrp18ddy7a" id="_effrp18ddy7a"></a>

In many cases, you want to see many metrics at once, list their exact values, and be able to sort those metrics. You can do this by adding or removing columns, or adding multiple filters to make it easier for you to find certain values.&#x20;

![](<../../.gitbook/assets/0 (9) (1)>)

The image above shows users what a Table looks like.

If you also want to summarize the grouping of rows or switch columns and rows, using a [Pivot Table](https://docs.footprint.network/getting-started/visualization/pivot-table) would be better.

### Line Charts <a href="#_r5y1ux7viix8" id="_r5y1ux7viix8"></a>

You may also often want to present data as a time series to see how a particular metric has changed over time, and you would use a line chart for in this case. A time series is any chart that involves tracking data by time, such as day, month or year. A line chart provides a simple shape for the data, making it easy to see if the numbers are trending up, or if they are cyclical, or what the maximum value was for the past X days, among other things.

![](<../../.gitbook/assets/1 (1)>)

The image above shows users what a Line Chart looks like.

Let’s walk through some common situations to help you choose the right visualization chart to show your findings.

### When You Only Have One Value <a href="#_2seca5fsa4u4" id="_2seca5fsa4u4"></a>

### Number Visualization <a href="#_7gs7jvikph8x" id="_7gs7jvikph8x"></a>

When you only have one value, especially for static numbers, or at least a number that doesn’t change too frequently, use the (appropriately named) [**Number Visualization**](https://docs.footprint.network/getting-started/visualization/numbers-and-trend), which is good for at-a-glance values.&#x20;

![](<../../.gitbook/assets/2 (3)>)

The image above shows an example of what Number Visualization looks like.

Keep in mind that a single number may lack context, so it’s best used on a dashboard that provides that context.

![](<../../.gitbook/assets/3 (1)>)

The image above shows an example of a Dashboard combining different charts together to provide context for your data.

### Comparing Metrics <a href="#_u44r1e43rjl" id="_u44r1e43rjl"></a>

Often, we want to see how multiple values stack up against each other. The most common comparisons are a single metric’s performance over time and a single metric across other dimensions.

### Static Comparisons <a href="#_cvkcmv8fn7bz" id="_cvkcmv8fn7bz"></a>

For measures that won’t change, like responses on a survey or an annual report, you can compare values with a [**Bar Chart**](https://docs.footprint.network/getting-started/visualization/master-the-bar-chart-visualization) (sometimes called a **Column Chart**). If you have a lot of different items you need to compare, you could try switching to a row chart to see if that makes the bars more legible for you.

![](<../../.gitbook/assets/4 (4)>)

The image above shows users an example of what a Bar Chart looks like.

### One Measure Over Time <a href="#_yd2prhw8r63s" id="_yd2prhw8r63s"></a>

When you want to compare and emphasize two sequential values of a metric, or have a number that can be broken down by time, you can use a [Trend Chart](https://docs.footprint.network/getting-started/visualization/numbers-and-trend). Trend Charts show the current value of the metric and the previous value of that metric at whichever interval you’re tracking it at.

![](<../../.gitbook/assets/5 (7)>)

The image above shows users an example of what a Trend Chart looks like.

If you don’t need to emphasize the most recent data, consider a time series instead, so that the shape of the metric over time can be seen. This is especially useful if the most recent data is uncharacteristic of larger trends. Trends are also great for situations in which teams need to look at a metric weekly and roughly know its behavior.

**Line charts** are the classic format for time series, but you can also present series values as a **Bar Chart** or an **Area Chart**.

### Multiple Measures Over Time <a href="#_gjvk0yypyk19" id="_gjvk0yypyk19"></a>

You can layer two time series on a line chart, with each line sharing the y-axis. If your measures have different scales or units of measurement, then you can use a combined graph with two different y-axes to highlight this difference.

![](../../.gitbook/assets/6)

This image shows users an instance where a chart has two y-axes, both showing different data being tracked despite them both revolving around a monthly basis.

### Showing The Relationship Between Measures <a href="#_sedo11oq6xbb" id="_sedo11oq6xbb"></a>

Sometimes you’ll want to see how two different measures correlate with each other.

The most basic way to see a relationship is to plot one variable along the x-axis and the other variable along the y-axis, and see if a pattern emerges. This graph is known as a [Scatter Plot Chart](https://docs.footprint.network/getting-started/visualization/scatter). You’ll often see scatter plots used with data that hasn’t been summarized or aggregated. Each dot on the chart represents an individual record in the data.

![](<../../.gitbook/assets/7 (5) (1)>)

The image above shows how each dot on the chart represents its own individual data separate from the other dots.

If you want to introduce a third variable, you could change the size of each dot to reflect the value of the additional variable, turning a scatter plot into a [**Bubble Chart**](https://docs.footprint.network/getting-started/visualization/scatter).

![](<../../.gitbook/assets/8 (4)>)

The image above shows users an example of a Bubble Chart.

### Breakouts <a href="#_jcecylmhu8ga" id="_jcecylmhu8ga"></a>

A breakout shows the composition of a measure. Breakouts are categories that make up a bigger set of data and can include **Pie Charts**, **Area Charts**, and **Bar Charts**.

### A Metric With Several Groups or Categories <a href="#_waa6b9yva6ry" id="_waa6b9yva6ry"></a>

[**Pie Charts**](https://docs.footprint.network/getting-started/visualization/pie) show how several parts make up a whole.&#x20;

![](<../../.gitbook/assets/9 (3) (1)>)

The above image is an example of a Pie Chart.

While the Line Chart is more suitable for data with a trend over time, the Pie Chart shows the percentage of a category in the whole. You could even use a [**Dynamic Pie Chart**](https://docs.footprint.network/getting-started/visualization/dynamic-pie-chart) to combine them both together. You can see how the values and pie charts change over time, instead of a new pie chart needing to be created every day.

![](<../../.gitbook/assets/10 (5) (1)>)

The gif above shows users how the values change over time in the graph as reflected by the Pie Chart.

### Categorical Breakouts Over Time <a href="#_vl0iaqgr3mo2" id="_vl0iaqgr3mo2"></a>

If you need to show how a number changes over time, and show the composition of that number at each interval, then consider using a [**Stacked Area Chart** or **Stacked Bar Chart**](https://docs.footprint.network/getting-started/visualization/area).

![](<../../.gitbook/assets/11 (4)>)

The above image is an example of a Stacked Bar Chart.

### Relative Changes Among Categories Over Time <a href="#_gcb69s1872ki" id="_gcb69s1872ki"></a>

If you need to see how different categories change relative to each other over time, regardless of the specific numbers, you could use percentages in your stacked bar charts.

![](<../../.gitbook/assets/12 (3) (1)>)

The image above shows the percentage option being used to represent the data on the y-axis in the Stacked Bar Chart.

There are so many different customization options and real-life uses for each of the mentioned types of charts. Explore for yourself and find out which charts work best for you [here](https://www.footprint.network/dashboards).
