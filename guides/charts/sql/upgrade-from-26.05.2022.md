# Upgrade from 26.05.2022

The upgraded Footprint is enhanced in the following aspects:

* High performance, high availability, high reliability
* support fast user and query growth
* modern MPP architecture ([Apache Doris](https://github.com/apache/doris))
* Support standard SQL language, compatible with MySQL protocol**.**

{% hint style="warning" %}
If you experiencing the errors during the execution of your SQL queries, please try using [MySQL](https://www.w3schools.com/sql/sql\_ref\_mysql.asp) dialect instead.
{% endhint %}

Changes in frequently used functions:

| Previously                        | Currently (standard SQL, MySQL syntax)                                | Example                                                                                                                                  |
| --------------------------------- | --------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| `current_timestamp`               | <p><code>current_timestamp()</code> and </p><p><code>now()</code></p> |                                                                                                                                          |
| `–`                               | `–“ ”`                                                                | <p><code>Select –day,tvl</code><br><code>* from xxx</code><br>change to<br><code>Select – day, tvl</code><br><code>* from xxx</code></p> |
| `data_trunc`                      | `DATE(date)` and `DATE_FORMAT (date, fmt)`                            |                                                                                                                                          |
| `string_agg`                      | `concat`                                                              |                                                                                                                                          |
| `distinct a group by a`           | `a group by a`                                                        |                                                                                                                                          |
| `date_diff (expr1, expr2, expr3)` | `date_diff (expr1, expr2)`                                            |                                                                                                                                          |
| `safe_cast()`                     | `cast()`                                                              |                                                                                                                                          |
| `float64`                         | `float`                                                               |                                                                                                                                          |
| `lag (expr, offset)`              | `lag (expr, offset, default)`                                         |                                                                                                                                          |
