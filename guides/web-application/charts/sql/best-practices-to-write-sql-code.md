# Best Practices to Write SQL Code

Good sql habits can improve the efficiency of running SQL, hope these cases can help you optimise your sql code and find the data you want faster.

## `WHERE` clause

Reduction of column conversions

### 🔴 Not recommended ****&#x20;

```
date(block_timestamp) > '2022-03-01'
```

### 🟢 Recommended&#x20;

```
block_timestamp > CAST ('2022-03-01' AS datetime)
```

## `SORT` clause

For the time of sorting, can be done in the last layer, do not need each layer of subquery are sorted on the time of sorting, midway `SORT` does not make much sense.

## Number of results

Try to `LIMIT` the time and order of magnitude of large tables at the beginning, filter only the required fields, and try to avoid full table scans.

### 🔴 Not recommended ****&#x20;

```
SELECT *
FROM TABLE
```

### 🟢 Recommended&#x20;

```
SELECT name,
       on_date
FROM TABLE
LIMIT 10
```

## `JOIN` clause

When join, put the small table on the **left side**, and each time you `JOIN` or `SELECT`, think about whether you can significantly reduce the amount of data.

## `IN` and `NOT IN` clauses

`IN` and `NOT IN` should also be used with caution, otherwise it will lead to a full table scan, for continuous values, `BETWEEN` can be used, do not use `IN`.
