# SQL

## Implementation

As it could be seen in [architecture.md](../../../architecture.md "mention")data is stored within the MySQL database. The appropriate dialect must be used when building SQL queries.

## Example

Let's build the same chart that was given as an example in [get-started-with-creating-a-chart.md](../get-started-with-creating-a-chart.md "mention"), but with SQL now.

**Step 1**. Click on <mark style="background-color:purple;">Create</mark> and select <mark style="background-color:purple;">SQL query</mark>

The image above shows users how to create a new chart based on Steps 1 and 2.

**Step 2.** Enter the following SQL query

```sql
SELECT
    `ethereum_transactions`.`block_date` AS `block_date`,
    count(*) AS `count`
FROM
    `ethereum_transactions`
GROUP BY
    `ethereum_transactions`.`block_date`
ORDER BY
    `ethereum_transactions`.`block_date` ASC
```

**Step 3**. Choose a <mark style="background-color:purple;">Line chart</mark> as a visualisation option
