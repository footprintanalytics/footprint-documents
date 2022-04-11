---
description: Guide to Number Visualization and Trend Chart.
---

# Numbers and Trend

When you only have one value, especially for static numbers, or at least a number that doesn’t change too frequently, use the (appropriately named) number visualization, which is good for at-a-glance values like the number of protocols on the Fantom chain.

Keep in mind that a single number may lack context, so it’s best used on a dashboard that provides that, such as Curve's TVL yesterday and the day before.

![](<../../.gitbook/assets/0 (3) (1)>)

#### **Numbers** <a href="#_kxwvyl9xtjdb" id="_kxwvyl9xtjdb"></a>

The Numbers option is for displaying a single number, nice and big. The options for numbers include:

* **Adding character prefixes or suffixes** to it (so you can do things like put a currency symbol in front or a percent at the end).
* **Setting the number of decimal places** you want to include.
* **Multiplying your result by a number** (like if you want to multiply a decimal by 100 to make it look like a percent). If you want to divide by a number, then just multiply it by a decimal (e.g, if your result is **1,000,000**, but you want it to display as **1M**, simply multiply it by **0.000001**).

#### **Trends** <a href="#_zhxtoul1wlqo" id="_zhxtoul1wlqo"></a>

The Trend visualization is great for displaying how a single number has changed over time. To use this visualization, you’ll need to have a single number grouped by a Time field, like the Count of Orders by Created At. The Trend will show you the value of the number during the most recent period, as well as how much the number has increased or decreased compared to its value in the previous period. The period is determined by your group-by field; if you’re grouping by Day, the Trend will show you the most recent day compared to the day before that.

![](<../../.gitbook/assets/1 (4) (1) (1)>)

By default, Trends will display increases as green (i.e. good) and decreases as red (bad). If your number is something where an increase is bad and a decrease is good (such as Bounce Rate, or Costs), you can reverse this behavior in the visualization settings:

![](<../../.gitbook/assets/2 (4)>)

**Use Case**

Let’s create a chart of Curve's TVL with number visualization and show the daily rate of change.

Step 1：Click on **Create** and select **New chart**. /Create your new chart.

Step 2：Search for **TVL** in the search box and select the data table **defi\_daily\_stats**

![](<../../.gitbook/assets/3 (4) (1) (1)>)

Step3：Click **Filter**, select **name**, search for **Curve** in the search box.

![](<../../.gitbook/assets/4 (2) (1)>)

Step 4: Click on **Summarize**, Footprint defaults to counting the records, click on **Count** and change it to **Sum of** and select the **TVL**.

Next, we’ll want to group the TVL by day. In the Group by section, mouse over the **Day** field, click on the **by day** to add the grouping, and click on **Done**.

![](<../../.gitbook/assets/5 (1) (1) (1) (1)>)

Step 5: Click on Visualization in the top right to bring up the Visualization sidebar. Choose Number, and select the **Field** to show as Sum of tvl.

![](<../../.gitbook/assets/6 (2) (1) (1) (1)>)

Step 6：If you need to remove the decimal places, you can set the minimum number of decimal places to **0**. To abbreviate 1000000 to 1M, you can multiply it by **0.000001**, and add the suffix **M**.

![](<../../.gitbook/assets/7 (1) (1) (1)>)

Step 7： Click **Visualization**, and choose **Trend**.

![](<../../.gitbook/assets/8 (1) (1)>)

Now, your number chart is done, don't forget to save your chart.
