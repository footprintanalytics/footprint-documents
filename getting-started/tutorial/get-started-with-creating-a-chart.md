---
description: >-
  This guide will help you create a visual chart on Footprint Analytics with 2
  basic examples.
---

# 🔎 Get Started with Creating a Chart

Footprint Analytics is a simple and powerful analytics tool which allows anyone to analyze on-chain data without technical requirements.

A basic chart is the first step to start the analysis.



**Example 1 - Using Template for a Chart**

By changing some settings or filters, you can quickly get the same chart as the template.

Let's create a Combo chart of $SOL: Token Price & Trading Volume per day.

Step 1: Click on **Create** and select **New chart**.

Step 2: Select the template **Avalanche: Token Price & Trading Volume**.

![](<../../.gitbook/assets/0 (1)>)

Step 3: Change the Filters in the upper left corner of the chart, change the filters to sol .

![](<../../.gitbook/assets/2 (2)>)

Then, the chart is done.

![](<../../.gitbook/assets/3 (2)>)

Step 4: Save chart, you can also change the chart name and add description.

**Example 2 - Using Dataset for a Chart**

Unlike one-click duplication, you need to create your own charts step by step. For creative graphs or data, this is a more flexible way to go.

Use case: Let's make a line chart of the number of Ethereum transactions per day.

Step 1: Click on **Create** and select **New chart**.

Step 2: Select the data table **ethereum\_transactions**.

![](../../.gitbook/assets/4)

Step 3: Since in the “ethereum\_transactions” table, there is one record for each transaction, you can directly count the number of records and group by day. Click **Summarize** in the upper right corner, pick Count of rows, and for group-by field choose **block\_timestamp** which needs to be grouped **by day**.

![](../../.gitbook/assets/5)

Step 4: You can see the line chart is ready, and then click **Done** to save this setting.

![](../../.gitbook/assets/6)

Step 5: Don't forget to save your chart.
