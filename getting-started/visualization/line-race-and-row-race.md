---
description: Guide to Create a Line Race and Row Race
---

# Line Race and Row Race

Line Race and Row Race are advanced applications of line charts, which can make your charts more vivid and visual.

* **Line Race**

It is used for plotting data captured in several sequences.&#x20;

![](<../../.gitbook/assets/0 (3)>)

**Use case:** Line Race - Comparison of Volumes

Step1: Select the data **nft-marketplaces-daily-stats** and add filters.

In this case, we make a comparison of trading volume of 3 NFT trading market in the past 30 days. So, we choose **protocol-name** and **day**.

![](<../../.gitbook/assets/1 (1)>)

![](<../../.gitbook/assets/2 (6)>)

Step2: Add summarize.

Here you can choose the metrics you need, then choose the field to group by. Note the choice of units for the time type field.

Click **Summarize**, in this case, we choose **sum of volume**, group by **protocol-name** and **day** (This operation displays data by day).

![](<../../.gitbook/assets/3 (1)>)

Step 3: Visualize.

Click **Visualize**, choose **Line Race**.Then, select the fields corresponding to x-axis, y-axis and category as required.

![](<../../.gitbook/assets/4 (4)>)

In this case, we choose:

X-axis = day;

Y-axis = sum of volume;

Category = protocol-name;

OK, the chart is done.

![](<../../.gitbook/assets/5 (2)>)

Save to complete the creation of the chart.

* **Row Race**

Row race sometimes is more suitable for multiple metrics than line race. Gives you a clearer view of how the rankings change for each metric.

![](<../../.gitbook/assets/6 (4)>)

**Use case:** Row Race - Comparison of Sum of tvl

Step1: Select the data **defi-daily-stats** and add filters.

In this case, we make a comparison of the sum of tv of 10 chain, the time is after March 31, 2021. So, we choose **chain** and **day**.

![](../../.gitbook/assets/7)

Step2: Add summarize.

Click **Summarize**, in this case, we choose **sum of tvl**, group by **chain** and **day** (This operation displays data by day).

![](<../../.gitbook/assets/8 (2)>)

Step 3: Visualize.

Click **Visualize**, choose **Row Race**.Then, select the fields corresponding to x-axis, y-axis and category as required.

![](<../../.gitbook/assets/9 (1)>)

In this case, we choose:

X-axis = sum of tvl;

Y-axis = chain;

Time = day;

![](<../../.gitbook/assets/10 (1)>)

And you can set the display to change Animation Speed, Y-axis Maximum and Y-axis Emphasize.

![](<../../.gitbook/assets/11 (1)>)

Then, your chart is done, don’t forget to save it.

Does this article work for you? If you have more advice and feedback for this tutorial, please feel free to give us your feedback in the community or contact us on Twitter or Telegram, we will try to do more and better.&#x20;

Click and tell us your idea! [Discord](https://discord.com/invite/3HYaR6USM7) [Twitter](https://twitter.com/Footprint\_DeFi) [Telegram](https://t.me/joinchat/4-ocuURAr2thODFh)
