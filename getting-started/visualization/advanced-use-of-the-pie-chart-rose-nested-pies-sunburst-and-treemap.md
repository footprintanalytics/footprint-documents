---
description: Advanced Use of the Rose Chart, Nested Pie, Sunburst Chart and Treemap
---

# Advanced Use of the Pie Chart Rose, Nested Pies, Sunburst and Treemap

Footprint Analytics offers users four styles of pie charts, allowing users to more flexibly and creatively customize and present their data as needed. The Rose Chart, Nested Pie, Sunburst Chart and Treemap are all somewhat related to their pie chart, the difference being that the Rose Chart and Nested Pie are used for two dimensional data, and Sunburst and Treemap are used for three dimensional data.

In this article:

* Rose Chart
* Nested Pie Chart
* Sunburst Chart
* Treemap Chart

### Rose Chart <a href="#_5fb07yuohqx7" id="_5fb07yuohqx7"></a>

The **Rose Chart** shows a more intense style for showing data percentage in one dimension. Each directional axis shows values increasing outwards

![The gif above demonstrates what a Rose Chart would look like upon hovering over it.](<../../.gitbook/assets/0 (7)>)

Let’s go through the process of making our own Rose Chart using the Sum of Users from Different Chains.

**Use case:** [**Rose - Sum of users of different chains**](https://www.footprint.network/chart/gamefi-daily-stats%2C-Sum-of-users%2C-Grouped-by-chain%2C-Filtered-by-day-fp-17242)****

Step 1: Click on **Create**, then click on **New Chart**.

Step 2: Click on GameFi from the list on the left of the screen, then select the data **gamefi\_protocol\_daily\_stats.**

Step 3: Click **Filter**. In this case, we will be focusing on a sum of users from different gamefi chains for the previous 7 days. So, click day and set the filter to **Previous 7 Days**. Click **Add filter**.

![The image above shows users where to find the day option under Filter based on Step 3.](<../../.gitbook/assets/1 (3)>)



![The image above shows users where to set the filter to Previous 7 Days and where the Add filter button is based on Step 3.](<../../.gitbook/assets/2 (5)>)



![The gif above demonstrates Step 3 on how to filter.](<../../.gitbook/assets/3 (8)>)



Step 4: Click **Advanced** on the top right corner of the screen. **** Click the **Summarize** button Click on **Pick the metric you want to see** and set it to **Sum of users**. Click on Pick a column to group by and set it to **chain**.

![The image above shows users where and what to summarize based on Step 4.](../../.gitbook/assets/4)



![The gif above demonstrates Step 4 on how to summarize.](<../../.gitbook/assets/5 (4)>)



Step 5: Click **Visualize**, then choose **Rose**. Then, set the data as required.

In our case, we will be leaving the **Name** as default and changing the **Numerical Value** from **chain** to **sum of users** using the downward arrow icon, then click **Done**.

![The gif above demonstrates how to switch your numerical value to the sum of users based on Step 5.](<../../.gitbook/assets/6 (8)>)



Step 6: Click on the **Display** tab next to **Data**. This is where you can set how your chart will be displayed.

![The gif above demonstrates how users can set their chart’s display as mentioned in Step 6.](<../../.gitbook/assets/7 (5)>)



Your chart is finally complete, just don’t forget to Save it.

### Nested Pie Chart <a href="#_50k147cju4bi" id="_50k147cju4bi"></a>

**Nested Pie Charts**, also known as a **Nested Donut Chart**, display the given data in multiple levels. Nested Pie Charts are used to show data percentages in two dimensions.

_**Note**: Nested Pie Charts are only available to membership holders._

![The gif above demonstrates what a Nested Pie Chart looks like upon hovering over it.](<../../.gitbook/assets/8 (8)>)



We will be using the Sum of TVL from different chains as an example to create our own Nested Pie Chart from the beginning.

**Use case:** [Nested Pies - Sum of tvl of different chains](https://www.footprint.network/chart/Nested-Pies-Sum-of-tvl-of-different-chains-fp-17394/notebook)

Step 1: Click on **Create**, then click on **New Chart**.

Step 2: Click on DeFi from the list on the left on the screen, then select the data **defi\_protocol\_daily\_stats**.

Step 3: Click on **Filter**. In this case, we are making a sum of tvl from three DeFi chains for yesterday. So, we choose **day,** then set it to **Previous 1 Day.** Click on **Add filter**.

![The image above shows users where to find the day filter based on Step 4.](<../../.gitbook/assets/9 (2)>)



![The image above shows users where and how to set the filter as yesterday based on Step 4.](<../../.gitbook/assets/10 (4)>)



![The gif above demonstrates filtering for yesterday based on Step 4.](<../../.gitbook/assets/11 (3)>)



Step 5: Click on **Advanced on the top right corner of the screen. Click on Summarize.** Click on **Pick the metric you want to see** and select **Sum of tvl**.Click on **Pick a column to group by** and select **chain** and **protocol\_name**.

![The image above shows where and what to summarize based on Step 5.](<../../.gitbook/assets/12 (3)>)



![The gif above demonstrates how and what to summarize based on Step 5.](../../.gitbook/assets/13)



Step 6: Click **Visualize**, then choose **Nested Pies**.Then, set the data as required.

In this case, we will be choosing **chain** for the Inner Type, **name** for the Outer Type, and **sum of tvl** for the Numerical Value by clicking on the downward arrow for the respective fields.

![The image above shows users where the Data Settings are based on Step 6.](<../../.gitbook/assets/14 (1)>)



![The gif above demonstrates how to set the data settings based on Step 6.](<../../.gitbook/assets/15 (3)>)



Step 7: Click on the **Display** tab next to **Data**. This is where you can set how your chart will be displayed.

![The gif above demonstrates where and how to set your chart display based on Step 7.](../../.gitbook/assets/16)



Don’t forget to save your chart.

### Sunburst Chart <a href="#_8x3v04zc5f39" id="_8x3v04zc5f39"></a>

**Sunburst Charts** are useful for visualizing hierarchical data structures. A sunburst chart consists of an inner circle surrounded by rings of deeper hierarchy levels. The angle of each segment is proportional to either a value or divided equally under its inner segment.

![The gif above demonstrates what a Sunburst Chart looks like upon hovering on it.](../../.gitbook/assets/17)



Let’s make our own Sunburst Chart using the sum of tvl from different chains.

**Use case:** [Sunburst - Sum of tvl of different chains](https://www.footprint.network/chart#eyJkYXRhc2V0X3F1ZXJ5Ijp7InR5cGUiOiJxdWVyeSIsInF1ZXJ5Ijp7InNvdXJjZS1xdWVyeSI6eyJzb3VyY2UtdGFibGUiOjE1MSwiYWdncmVnYXRpb24iOltbInN1bSIsWyJmaWVsZCIsMTY0MCxudWxsXV1dLCJicmVha291dCI6W1siZmllbGQiLDE2MjEsbnVsbF0sWyJmaWVsZCIsMTYyMyxudWxsXSxbImZpZWxkIiwxNjQxLG51bGxdLFsiZmllbGQiLDE2MjAseyJ0ZW1wb3JhbC11bml0IjoiZGF5In1dXX0sImZpbHRlciI6WyJhbmQiLFsidGltZS1pbnRlcnZhbCIsWyJmaWVsZCIsImRheSIseyJiYXNlLXR5cGUiOiJ0eXBlL0RhdGVUaW1lV2l0aExvY2FsVFoifV0sLTEsImRheSJdLFsiPiIsWyJmaWVsZCIsInN1bSIseyJiYXNlLXR5cGUiOiJ0eXBlL0Zsb2F0In1dLDUwMDAwMDAwMF0sWyJkb2VzLW5vdC1jb250YWluIixbImZpZWxkIiwiY2hhaW4iLHsiYmFzZS10eXBlIjoidHlwZS9UZXh0In1dLCJFdGhlcmV1bSIseyJjYXNlLXNlbnNpdGl2ZSI6ZmFsc2V9XV19LCJkYXRhYmFzZSI6M30sImRpc3BsYXkiOiJzdW5idXJzdCIsImRpc3BsYXlJc0xvY2tlZCI6dHJ1ZSwidmlzdWFsaXphdGlvbl9zZXR0aW5ncyI6eyJzdW5idXJzdC51c2VDZW50ZXIiOnRydWUsImNpcmNsZS5jb2xvciI6IiM3MTcyQUQiLCJzdW5idXJzdC5kYXRhIjoic3VtIiwidHJlZW1hcC5mb3VyIjoic3VtIiwidHJlZW1hcC5kYXRhIjoic3VtIiwiY2lyY2xlLnR3byI6ImNhdGVnb3J5Iiwic3VuYnVyc3Quc2hvd1BlcmNlbnRhZ2UiOmZhbHNlLCJjaXJjbGUuZm91ciI6InN1bSIsInRyZWVtYXAub25lIjoiY2hhaW4iLCJzdW5idXJzdC5mb3VyIjoic3VtIiwidHJlZW1hcC50d28iOiJjYXRlZ29yeSIsInN1bmJ1cnN0LnR3byI6ImNhdGVnb3J5IiwidHJlZW1hcC50aHJlZSI6Im5hbWUiLCJjaXJjbGUudGhyZWUiOiJuYW1lIiwic3VuYnVyc3Quc2hvd051bWVyaWNhbCI6ZmFsc2UsImNvbHVtbl9zZXR0aW5ncyI6eyJbXCJuYW1lXCIsXCJzdW1cIl0iOnsic2NhbGUiOjFlLTksInN1ZmZpeCI6IkIifX0sInN1bmJ1cnN0Lm9uZSI6ImNoYWluIiwic3VuYnVyc3QudGhyZWUiOiJuYW1lIiwiY2lyY2xlLm9uZSI6ImNoYWluIiwibmVzdGVkcGllcy5pbm5lciI6ImNoYWluIiwibmVzdGVkcGllcy5vdXRlciI6Im5hbWUiLCJuZXN0ZWRwaWVzLmRhdGEiOiJzdW0ifSwib3JpZ2luYWxfY2FyZF9pZCI6MTY2NzJ9)

Step 1: Click on **Create**, then click on **New Chart**.

Step 2: Click on **DeFi** from the list on the left on the screen, then select the data ud\_**defi\_token\_growth**.

Step 3: Click on **Filter**, click on **day**, then set to **Previous 1 Day**. Click on **Add filter**.\


![The image above shows users where to filter for a day based on Step 3.](<../../.gitbook/assets/18 (2)>)



![The image above shows filtering for Previous 1 Day is equivalent to yesterday based on Step 3.](<../../.gitbook/assets/19 (2)>)



![The gif above demonstrates Step 3 of setting the filter to yesterday.](<../../.gitbook/assets/20 (1)>)



Step 4: Click on **Filter**. Select **sum of tvl,** then set it to greater **than 500,000,000**. Click on **Add filter**.

![The image above shows users to scroll down for tvl under filter based on Step 4.](https://lh3.googleusercontent.com/NgRYxP8ioFalOqWBefAtRh3YQ4PH8dZ6rcCC324MEexJB\_NmmkIbFucz-uPAsLNfP8dpr9EIwNnNVTrEpAdzyWljCUFkRPAs3TLFTKsNQFSYXrNfNour-kYPQW73Ay\_dOEdnU9RIEs23Lp8EoA)

![The image above shows users how to filter for tvl values based on Step 4.](https://lh6.googleusercontent.com/5jRSR7636iPc-6GhqHO5yXf\_FxWzlQc\_6NwTWCO7k3770safxr4OOQieRakW2FYw86gS5zXF1iJ6h3rW4cNkBhJyqPl3F1PFX4WqeGrwsb50Th8pdq0uItIF6XHKnhVcR-HMJJ89SPHPRLR6zw)

![The gif above demonstrates how to set your tvl values under filter in Step 4.](https://lh5.googleusercontent.com/9qUAHzX98SveMOjW2LgMzFAp\_UYRRRrWgEiKqzEwiRSCvmUWNZBh7oYZP\_VPmYHRv0odxqnLMRMDMPZ\_8eYjcgU5WReYcVjn3yivwBXO0zZro2dnu0L73dgsEPeyiOrTiV3ExjqSBUbmnwHasQ)



Step 5: Click on **Filter**. Select **chain**, In this case, we set it to **does not contain** and type in **Ethereum**，to show the distribution of other public chains. Since Ethereum would take over 60% of the chart, it would be difficult to identify the data for the other chains on the chart if Ethereum were added, so for our case, we will be excluding it. **** Click on **Add filter**.

![The image above shows users where to filter for chains based on Step 5.](https://lh6.googleusercontent.com/K47bbIGv7xNSftvjypgfCNnSd5pR8AmQ0iGCyCWs89Nvr8syKusmQJwVqH7YFFXKxiPnqz4YmAkpMppXADR5hohVdueRdRleJf-VHyA0u0CQj4qxZD8GfOSGnH3v92n08N9C9d5IihqYOHkE-g)

![The image above shows users how to filter through data that does not contain Ethereum based on Step 5.](https://lh6.googleusercontent.com/7KGC6tc6ukxC8A0v-ICSpSkOQ9LDMPitaREsOWAt9WRB9mwwiP3jaeAyo6nu7S918jzoBHJ5q9ZuN7WV1gr9zevrb8DajZcc4XWlKXZ38RCBb5vIN8RatgYgeqz9V-EFzghhcxHXU-Z3r1zbUA)

![The gif above demonstrates how to set your chart to not contain Ethereum based on Step 5.](https://lh6.googleusercontent.com/swRzN4c8uWi7cEny4Vg3TV89SriwpJmvOTQ1PZcVSbo0gLLhiYRyj58pECwycpAmQtO-pWOr6WmaFKtVYYiYD0JdXOEB1ZQsbsxBuMI\_CUH1hUGVWBu-mvnbYpFkKQbJxCFRBSYTyDgs6gAXdg)



Step 6: Click on **Advanced** on the top right corner of the screen. Click on **Summarize**. **** Click on **Pick the metric you want to see** and select **Sum of tvl**. Click on **Pick a column to group by** and select **chain, category, name** and **day**.&#x20;

![The image above shows users how and what to summarize based on Step 6.](https://lh3.googleusercontent.com/0mPZ20\_uiIg6qWy6HaxPKYEepEgMlAwxE80HIl\_aYhC2T1ithp24ty\_xZqAjRDFe8QKAA61W5t6qhy9qkl\_-p0kYsH68GBOOAgZOqQ-f3wdJKPXzqIgil6cZGvVF\_z\_q2Le3\_EAN9mLynaK3pg)

![The gif above demonstrates how and what to summarize in Step 6.](https://lh3.googleusercontent.com/yar\_sgbUR14T0hVfHdfpRljvflzJFQEbdRhWSrxj6755PgiKabJ9eM9Pj9Hjf3HZHPn8Qy6my\_5H9rPhhZKy0OX4fCyydAjwgQAmCo1fX0kNZd9niLNm00lGDQ3MT6bzfzUVfxvQtFbCUmXNsA)



Step 7: Click **** on **Advanced,** then click on **Visualize** and choose **Sunburst**. Setting the data as required.

For our example, set **chain** as the First Level, **category** for the Second Level, **name** for the Third Level, and **Sum of tvl** for the Numerical Value by clicking on the downward arrow for the respective fields.

![The gif above demonstrates where to set the data for your chart based on Step 7.](https://lh4.googleusercontent.com/hnfhbceUekmNYkBxcnbWwnRa8DydwoQt2tgvMGTThNH7uO\_bFQxKLEw73CjDDNNf5gh0VGBcy8Bsq2MgJnktZee-C1CqPZsLa\_SLovuWmFm9cJ0w7G3hX-h3CbKANmnpgH3ZR1FtSNtW2Umbfg)



Step 8: Click on the **Display** tab next to **Data** to set how you want your chart to look.

![The gif above demonstrates where and how to set your display based on Step 8.](https://lh5.googleusercontent.com/4hURgANF2A69rEw8F5GrOC1-pLEqkC0JaYTz8cUMygjmohYYXzq9LuDSLQuOSVGW8AmtVN0CwMu3Nl-exyuUDRDthsYA5Es-sObV-wFMuKmlcKKBzVrfG6OCxqz4rEqhdi5RdPgKz4W6g9AsYg)



Always save your chart.

### Treemap Chart <a href="#_4fug9snbfge8" id="_4fug9snbfge8"></a>

Treemaps are used for showing data percentage in three dimensions. Treemaps capture relative sizes of data categories, allowing for quick perception of the items that are large contributors to each category by the shade of color. Color can identify items that are underperforming or over performing compared to their siblings from the same category.

Let’s create our own Treemap based on the sum of tvl from different chains.

**Use case:** [Treemap - Sum of tvl of different chains](https://www.footprint.network/chart/treemap-sum-of-tvl-of-different-chains-fp-17258)

![The gif above demonstrates what a Treemap looks like and how to use it.](https://lh4.googleusercontent.com/CW1CfXd13qvys5ymQtCHGjyoPhy7t00ESxd3rdblSqNWDXB2m8iOfWIe3XW0dKrpDpEOC5XoMDi1wmivrsMO94pD02X9Dhc1YwKcaZ4JT3wBW9839ixR\_60zNdT7J\_TLxURcLStKZOTFvK96MA)

Step 1: Click **Create** and then click **New Chart**.

Step 2: Click on **DeFi** from the list on the left of the screen. Select the data **ud\_defi\_token\_growth**.

Step 3: Click on **Filter**. Click on **day**, then set it to **Previous 1 Day** since we are making a sum of tvl of different chains for yesterday.

![The image above shows where to find day in filter based on Step 3.](https://lh6.googleusercontent.com/g0NVcTL5nLKjoiScWhUwiwJPZqwSa7UCf6tTxxQFduPoQc2g2Xur4Kn8mI1orv\_Q1I8FJgQfKEIpJHgpPKvrje4LwYEUQaS9kg9Vo73pQ-O2qZ1n2kdzT65lmlAie1ClVvGF-4Pe-CJHj-mTvQ)

![The image above shows where and how to set the filter to yesterday from Step 3.](https://lh4.googleusercontent.com/Ms7LCrW3R2B4xJt4uY3jBEaQcGFWCM91-dD5GGiZcoow0EPsjmEomdtCEWudFFCkKbij0y3xJXv5Bw0PgOpDZondnGXe24cBIG9w86cFH98ARy9HMuEq9A4taL6sBJnUNAsFts6SLPeKI0OoDA)

![The gif above demonstrates Step 3 of filtering by yesterday.](https://lh5.googleusercontent.com/CwixPPzzN5gsdcbsRGVC1ALN7pRPDRAxMuCIQuisM32H--aKSGW3xOOIVTsqa2xQ1fffPYkpXZqNyIEc4KDWmU72ITjg6EedbM7fYvVnlgYNBjddUGspsLXC6hK92zBClNZflRPs4KOTUH7MJA)



Step 4: Click on **Filter**. Click on **chain,** set it to **not empty,** then set **category** to not empty as well.

Step 5: Click **Advanced,** then click **Summarize**. Click on **Pick the metric you want to see** and select **Sum of tvl**. Click on **Pick a column to group by** and select **chain, category, name** and **day**.

![The image above shows what your data, filters and summarizations should look like after following Steps 1 to 5.](https://lh5.googleusercontent.com/qQUb711LcLj5lTpnbf4-zozLgTAdXMvjrgKFydakFxxuAWz5ehnvm3hk7eR0O\_j4gsKT65JzMOrFKrZKjfBjvioxNogRO97lh-2MwMSH35gU-kgBSoR6FgdHabTPCvuKJuNK3vjcvTYzvLWVrA)



Step 6: Click **Visualize**, then choose **Treemap**. Set your data as required.

In this case, we will be setting the First Level as chain, the Second Level as category, the Third Level as name, and the Numerical Value as Sum of tvl by clicking on the downward arrow for the respective fields.

![The gif above demonstrates what and where to set the chart data based on Step 6.](https://lh4.googleusercontent.com/Dde4uJ83AZsvgEbEmxCuBzebytVx1Y4xhSvOYzbiULaleFbdxTgo-6NUQQpUIxpVx7t4fzvt41xOnBHj\_FBVQkCC4m\_4jBDIrMsXBmOvyyedCkCDjGRp7iJx6Y9mcIXHeL\_9TVzaUF8d-cDlVQ)



Step 8: Click on the **Display** tab next to **Data** to set how you want your chart to look.

![The gif above demonstrates where and how to set your display based on Step 8.](https://lh6.googleusercontent.com/pSp6UhvuqZv\_RBAdwJxPAEEBrCb3FyBil122OAnxYXFUSFWWd7WOT5tjJ12kTq9KSIp-q19iuLeZ5R6olQ\_AFZcDCxI2GMxGVk5H1dcuw-STgftIdf7AHW4rO6LpTM4AP5uaQP5yNxJ8AlUw6g)



Your chart is done, don’t forget to save it.

Was this article helpful for you? If you have any advice or feedback for this tutorial, please feel free to let us know in the community or contact us on [Twitter ](https://twitter.com/Footprint\_DeFi)or [Telegram](https://t.me/joinchat/4-ocuURAr2thODFh). [Here](https://www.footprint.network/dashboards) at Footprint Analytics, we always aim to improve user experience.
