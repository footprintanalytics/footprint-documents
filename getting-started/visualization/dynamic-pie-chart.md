---
description: Dynamic Pie Chart Operation Tutorial
---

# Dynamic Pie Chart

While the Line Chart is suitable for data with a trend over time, the Pie Chart shows the percentage of a category in the whole, and the Dynamic Pie Chart combines them both.In Dynamic Pie Chart, you can visualize the trend of an metric's value and trend of its distribution over a certain time frame.You can see how the values and pie charts change over time,instead of a new pie chart created every day.

![](<../../.gitbook/assets/0 (4)>)

**Use case:** Dynamic Charts - TVL of Different Chains

Step1: Create a new chart.

Select the data **defi-daily-stats**.Then click **Advanced.**

![](<../../.gitbook/assets/1 (5)>)

Step2: Add filters.

Here you can filter the data, select the data interval, the type, etc you need.

Click **Filter**, in this case, we choose **day** and **chain**.(day-Previous 30 Days, chain-Algorand, Arbitrum,Astar, Aurora, Avalanche, Binance, CSC)

![](<../../.gitbook/assets/2 (6) (1)>)

Step3: Add summarize.

Here you can choose the metrics you need, then choose the field to group by. Note the choice of units for the time type field.

Click **Summarize**, in this case, we choose **sum of tvl**, group by **chain** and **day** (This operation displays data by day).

![](<../../.gitbook/assets/3 (4) (1)>)

Step4: Sort field.

This operation is so that the data can be sorted in chronological order, name or others.When you select the name sort, the arrow up means the data is sorted from smallest to largest, and the arrow down means the opposite.If you choose the time sort, it is similar.

Click **Sort**, in this case, we choose **Sum of tvl** and **day**.

![](<../../.gitbook/assets/4 (2)>)

Step 5: Visualize.

Click **visualize**, choose **Dynamic Pie**.Then, select the fields corresponding to x-axis, y-axis and category as required.

![](<../../.gitbook/assets/5 (2) (1)>)

In this case, we choose:

x-axis = day;

y-axis = sum of tvl;

category = chain;

![](<../../.gitbook/assets/6 (3) (1)>)

Save to complete the creation of the chart.

**Tips: Dynamic Pie Chart is used to filter at least two metrics, if you only have one metric, it will be meaningless.**
