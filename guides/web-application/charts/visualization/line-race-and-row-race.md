---
description: How to Create a Line Race and Row Race
---

# Line and Row Races

Line Race and Row Race are advanced applications of line charts. They provide and present your data in different ways, which can make your charts more vivid and visual. The main difference that sets them apart from line charts and most other charts, is that they are animated to help better show the process and progress of the data.

This article will guide you through Line Races and Row Races as well as walk you through some use cases.

### Line Race <a href="#_at8t0ip1t34l" id="_at8t0ip1t34l"></a>

Line Races are used for plotting data captured in several sequences.

![The gif above demonstrates an example of a line race as time goes by.](<../../../../.gitbook/assets/0 (14)>)

Use case: \*\*\*\* Line Race - Comparison of Volumes

Step 1: Click Create on the top right corner of the screen. A pop-up menu will appear. Click on New Chart.

Step 2: Click on NFT from the list on the left. Select **nft-marketplaces-daily-stats.**

Step 3: In this case, we will be making a comparison of the _trading volume of 3 NFT trading markets in the past 30 days_. Click on **Filter**, then click on **protocol\_name**. Search and select **OpenSea**, **X2Y2**, and **LooksRare**, then click **Add filter**.

![The image above shows where to find the protocol\_name under Filter.](<../../../../.gitbook/assets/1 (18)>)

![The image above shows the three protocol\_names we will be using for our example.](<../../../../.gitbook/assets/2 (17)>)

![The gif above demonstrates Step 3 in filtering by protocol\_name.](<../../../../.gitbook/assets/3 (10)>)

Step 4: Click on **Filter**, and this time click on **day**.

![The image above shows where to find the day option under Filter.](<../../../../.gitbook/assets/4 (15)>)

Step 5: Select **Previous**, **30** and **Days**, then click on **Add filter**.

![The image shows what the filter selection would look like for Step 5.](<../../../../.gitbook/assets/5 (1)>)

![The gif above demonstrates how to filter by the previous 30 days based on Step 5.](<../../../../.gitbook/assets/6 (4)>)

Step 6: Click on Advanced, then click on Summarize..

Step 7: Here you can choose the metrics you need, then choose the field to group by. Click on the **Pick the metric you want to see** button. Select **sum of**, then select **volume**.

Step 8: Click on the **Pick a column to group by** button. Select **protocol\_name**. Click on the green **+ button** and select **day,** and then select **by day** (This operation displays data by day).

Step 9: Click on **Visualize** on the bottom left corner of the screen.

![The image above shows users how to summarize their data under the Advanced tab.](<../../../../.gitbook/assets/7 (15)>)

![The gif above demonstrates Steps 7 and 8 in using the Summarize function.](<../../../../.gitbook/assets/8 (6) (1)>)

Step 3: Under **Visualization**, choose **Line Race**.Then, select the fields corresponding to x-axis, y-axis and category as required. Click on **Done**.

![The image above shows users where to find the Line Race option under Visualization.](../../../../.gitbook/assets/9)

In this case, we choose the following settings for our chart:

X-axis = day;

Y-axis = sum of volume;

Category = protocol-name.

![The image above shows how our completed Line Race chart would look like.](<../../../../.gitbook/assets/10 (6)>)

_**Note**: The Line Race chart is only available for membership holders._

Save to complete the creation of the chart.

### Row Race <a href="#_hsu6ddk5iop" id="_hsu6ddk5iop"></a>

Row races are sometimes more suitable for multiple metrics than line races. It gives you a clearer view of how the rankings change for each metric.

![The image above shows an example of what a Row Race looks like.](<../../../../.gitbook/assets/11 (3)>)

Use case: Row Race - Comparison of Sum of TVL

Step 1: Click on **Create**, then click on **New Chart**.

Step 2: Select the data **defi-daily-stats** under the **DeFi** drop-down list found on the left side of the screen.

Step 3: In this case, we will be making a comparison of the sum of TVL using 10 chains after March 31, 2021. Click on **Filter** on the top right corner, and then click on **chain**. Search and select the **chains Heco, Solana, PolyNetwork, Tron, Fantom, Stacks, Kava, Avalanche, Optimism,** and **Celo.**

![The image above shows users where to find the chain filter based on Step 3.](<../../../../.gitbook/assets/12 (6)>)

Step 4: Click on **Filter**, and then day. Select **After** and choose **May 31, 2021** for our example.

![The image above shows users where the day filter from Step 4 can be found.](<../../../../.gitbook/assets/13 (7)>)

![The image above shows users where to select their desired date using the calendar based on Step 4.](../../../../.gitbook/assets/14)

![The image above shows users what it looks like after the two filters from Steps 3 and 4.](<../../../../.gitbook/assets/15 (2)>)

Step 5: Click on Advanced, then click on Summarize. In our case, we will be selecting **sum of tvl**, grouped by **chain** and **day** (This operation displays data by day).

![The image above shows users where to summarize based on Step 5.](<../../../../.gitbook/assets/16 (1)>)

Step 6: Under Visualize, click **Visualization**, choose **Row Race**.Then, select the fields corresponding to x-axis, y-axis and category as required. Click on **Done**.

![](<../../../../.gitbook/assets/17 (1)>)

In this case, we choose the following settings for our chart:

X-axis = sum of tvl;

Y-axis = chain;

Time = day;

![](<../../../../.gitbook/assets/18 (1)>)

You can change the Animation Speed under the **Display Settings**, using the Y-axis Maximum and Y-axis Emphasize fields to customize.

![](../../../../.gitbook/assets/19)

Your chart is done, don’t forget to save it.
