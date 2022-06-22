---
description: Guide to Pivot Tables
---

# Pivot Tables

A pivot table is a data visualization tool that summarizes rows and columns of a table and lets you rotate (“pivot”) the columns to view those summaries in different ways. The summary rows are usually subtotals or grand totals, but they can also be other metrics such as averages and summations. This article will walk you through the creation and use case of a pivot table.

### Creating a Pivot Table <a href="#_py3gafnigb7t" id="_py3gafnigb7t"></a>

For this article, we will be using the Sum of TVL using different chains for our example in creating a pivot table.

Use case: **** [Pivot Table - Sum of tvl of different chains](https://www.footprint.network/chart/Use-case%3A-Pivot-Table-Sum-of-tvl-of-different-chains-fp-17534)

Step 1: Click on **Create**, and then click on **New Chart**.

Step 2: Select the data **defi\_protocol\_daily\_stats**.

Step 3: Click **Filter** on the top right corner, then click **chain**. In this case, we will be making a sum of tvl using different DeFi chains for the previous three days. So for our example, search and select Boba, CSC, and Celo. Click **Add filter**.

![](<../../../.gitbook/assets/0 (10)>)

The image above shows where to find the chain filter based on Step 3.

![](<../../../.gitbook/assets/1 (12)>)

The image above shows the three chains we filtered for: Boba, CSC and Celo.

Step 4: Click on Filter, and this time, choose a day. Set the filter to **Previous 3 Days**. Click **Add filter**.

![](<../../../.gitbook/assets/2 (6)>)

The image above shows where to find the day filter based on Step 4.

![](<../../../.gitbook/assets/3 (3)>)

The image above shows the filters chosen based on Step 4.

![](<../../../.gitbook/assets/4 (5)>)

The gif above demonstrates Steps 3 and 4.

Step 5: Click **Advanced** on the top right corner, and click on Summarize. Click on the **Pick the metric you want to see** button and select **Sum of tvl**. Click on Pick a column to group by button and select **chain,** then **day**, **** and **protocol\_name**.

![](<../../../.gitbook/assets/5 (5) (1)>)

The image above shows Step 5 of clicking Advanced and Summarize.

![](<../../../.gitbook/assets/6 (9)>)

The gif above demonstrates what and where to summarize in Step 5.

![](<../../../.gitbook/assets/7 (7)>)

The image above shows the end results of selecting the data set, filters, and what to summarize by.

Step 6: Click on **Visualize**, then select **Pivot Table**.

You will see the default settings:

Fields to use for the table rows = chain, name; (default)

Fields to use for the table columns = day;

Fields to use for the table values = Sum of tvl;

![](<../../../.gitbook/assets/8 (2) (1)>)

The gif above demonstrates Step 6 of clicking Visualize and selecting Pivot Table.

### Settings <a href="#_acfgvchavk9l" id="_acfgvchavk9l"></a>

### Rearranging Rows and Columns <a href="#_bk4nlir6slwq" id="_bk4nlir6slwq"></a>

To **rotate** the table, you can move the three fields, **rows, columns, and values**, around by **clicking and dragging** them **above and below** each other. This can be done across the other categories as well. The chart will update accordingly.

![](<../../../.gitbook/assets/9 (2)>)

The gif above demonstrates moving a field across the two categories rows and columns.

![](<../../../.gitbook/assets/10 (5)>)

The gif above demonstrates moving a field within the same category of rows.

### Toggling SubtotalsYou can toggle subtotals on and off by: <a href="#_y5vima65nngz" id="_y5vima65nngz"></a>

Step 1: Click on Setting.

Step 2: Click on the downward arrow to expand a category. In our example below, we expanded chain under rows.

### Step 3: Click on the toggle button next to the text Show totals. <a href="#_y5vima65nngz" id="_y5vima65nngz"></a>

![](<../../../.gitbook/assets/11 (1)>)

The gif demonstrates where you can find and how you can toggle showing totals under Setting based on Step 2 and 3.

### Collapsing and Expanding Groups of Rows <a href="#_wbetvfs9uz10" id="_wbetvfs9uz10"></a>

You can navigate the table by collapsing and expanding **groups of rows**. To expand a group of rows, just click on the **downward arrow** next to your desired field in your table. To collapse a field, click on the **upward arrow** next to a field in your table.

![](<../../../.gitbook/assets/12 (6)>)

The gif above demonstrates expanding and collapsing a group of rows by using the arrows.

### More Options <a href="#_ucubs5sapgyi" id="_ucubs5sapgyi"></a>

Each of the categories under Setting has their own additional options you can customize. To access them:

Step 1: Click on the **downward arrow** of your desired category.

Step 2: Click on **See options** next to the text **Formatting** to bring up more settings.

![](<../../../.gitbook/assets/13 (3)>)

The image above shows users where they can find the See options button.

![](<../../../.gitbook/assets/14 (3)>)

The gif above demonstrates where to find the See options button and an example menu of the kinds of settings it pulls up.

Don’t forget to click Save after setting up your pivot chart.
