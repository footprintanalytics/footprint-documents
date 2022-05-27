# How to Create Native Query

Hello\~ Footprint has been upgraded on May 26, 2022.



The upgraded Footprint will be enhanced in the following aspects:

* High performance, high availability, high reliability
* Support fast user and query growth
* Modern MPP architecture ([Apache doris](https://www.google.com/url?q=https://github.com/apache/incubator-doris\&sa=D\&source=editors\&ust=1653564029282616\&usg=AOvVaw3xcBmlMwQ-ySZj7dVFdNQQ))
* Support standard SQL language, compatible with MySQL protocol

For those woo have problems with SQL error, please use MySQL function instead. [link for MySQL function reference](https://www.google.com/url?q=https://www.w3schools.com/sql/sql\_ref\_mysql.asp\&sa=D\&source=editors\&ust=1653564029283842\&usg=AOvVaw1ZgS-n5wwqg\_aMOCOJnTJy)&#x20;

Changes to functions that we know are frequently used.

| **Previous**                  | **Current(standard SQL, MySQL syntax)** | **Example/Link**                                                                     |
| ----------------------------- | --------------------------------------- | ------------------------------------------------------------------------------------ |
| current\_timestamp            | <p>current_timestamp()</p><p>now()</p>  |                                                                                      |
| –                             | –“ ”\[a]                                | <p>Select –day,tvl<br>* from xxx<br>Change to<br>Select – day, tvl<br>* from xxx</p> |
| data\_trunc                   | DATE(date) and DATE\_FORMAT(date, fmt)  |                                                                                      |
| string\_agg                   | concat                                  |                                                                                      |
| distinct a group by a         | a  group by a                           |                                                                                      |
| date\_diff(expr1,expr2,expr3) | date\_diff(expr1,expr2)                 |                                                                                      |
| safe\_cast()                  | cast()                                  |                                                                                      |
| float64                       | float                                   |                                                                                      |
| lag(expr, offset)             | lag(expr, offset, default)              |                                                                                      |

\[a]you need a space between -- and other
