---
description: Create your own charts step by step with simple UI
---

# No code

## Implementation

To create a simple workflow with easy-to-use interface, we use [Metabase](https://www.metabase.com/). It handles the complexity of joins, aggregations, and more, freeing the users to focus on uncovering their next insight, rather than picking through long SQL.

## Example

Let's make a [guide-to-line-chart.md](visualization/guide-to-line-chart.md "mention") of _the number of Ethereum transactions per day_.

**Step 1**. Click on <mark style="background-color:purple;">Create</mark> and select <mark style="background-color:purple;">New chart</mark>.

![](../../../.gitbook/assets/11)

The image above shows users how to create a new chart based on Steps 1 and 2.

**Step 2.** Select <mark style="background-color:purple;">Ethereum</mark>. A drop-down menu will appear.

**Step 3**. Select the data table `ethereum_transactions`.

![](<../../../.gitbook/assets/13 (1)>)

The gif above demonstrates Steps 1 to 3, the process of getting to `ethereum_transactions` for the purpose of this guide.

**Step 4.** In the `ethereum_transactions` table, there is one record for each transaction, which means you can directly count the number of records and group by day. Click <mark style="background-color:purple;">Summarise</mark> \*\*\*\* in the upper right corner, and then pick <mark style="background-color:purple;">Count of rows</mark>.

![How to summarize by count of rows according to Steps 1 to 3.](<../../../.gitbook/assets/14 (3)>)

**Step 5**. Under the `ethereum_transactions` field, scroll down and select `block_timestamp`, which needs to be grouped `Day`.

![Scroll down for block\_timestamp under the Group-by field for Step 4.](../../../.gitbook/assets/15)

![Steps 4 to 5, navigating how to select Count of rows and block\_timestamp by day.](<../../../.gitbook/assets/17 (2)>)
