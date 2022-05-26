# How to create native query

Hello\~ Footprint has been upgraded(2022-05-26).

* The upgraded Footprint will be enhanced in the following aspects:
* High performance, high availability, high reliability
* support fast user and query growth
* modern MPP architecture([Apache doris](https://www.google.com/url?q=https://github.com/apache/incubator-doris\&sa=D\&source=editors\&ust=1653564029282616\&usg=AOvVaw3xcBmlMwQ-ySZj7dVFdNQQ))
* Support standard SQL language, compatible with MySQL protocol

Please report any issues at footprint [support channel](https://www.google.com/url?q=https://discord.com/channels/864829036294307881/864835552041631774\&sa=D\&source=editors\&ust=1653564029283317\&usg=AOvVaw2n3dRLIWgo40Mo7jK6Xn11). We apologize for any inconvenience this may cause, and we promise to do our best to complete this task perfectly in the shortest time possible.

For those we have problems with SQL error, please use MySQL function instead. [link for MySQL function reference](https://www.google.com/url?q=https://www.w3schools.com/sql/sql\_ref\_mysql.asp\&sa=D\&source=editors\&ust=1653564029283842\&usg=AOvVaw1ZgS-n5wwqg\_aMOCOJnTJy)&#x20;

Known functions(frequent used) change:

| previous                      | current(standard SQL, MySQL syntax)    | example/link                                                                         |
| ----------------------------- | -------------------------------------- | ------------------------------------------------------------------------------------ |
| current\_timestamp            | <p>current_timestamp()</p><p>now()</p> |                                                                                      |
| –                             | –“ ”\[a]                               | <p>Select –day,tvl<br>* from xxx<br>Change to<br>Select – day, tvl<br>* from xxx</p> |
| data\_trunc                   | DATE(date) and DATE\_FORMAT(date, fmt) |                                                                                      |
| string\_agg                   | concat                                 |                                                                                      |
| distinct a group by a         | a  group by a                          |                                                                                      |
| date\_diff(expr1,expr2,expr3) | date\_diff(expr1,expr2)                |                                                                                      |
| safe\_cast()                  | cast()                                 |                                                                                      |
| float64                       | float                                  |                                                                                      |
| lag(expr, offset)             | lag(expr, offset, default)             |                                                                                      |

\[a]you need a space between -- and other
