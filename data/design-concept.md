# Design concept

## **Data model**

Building ETL processes for blockchains involves processing huge amounts of unstructured data. Accordingly, designing a database is a non-trivial task. In the initial design of the data model, we pursued the following goals:

1. **Reduce the number table joins**. With the most frequently used combination of slug+chain, you can quickly find the data you want in multiple tables.
2. **Reduce the cost of understanding**. Consistent presentation of multiple fields in different tables, reduces the cost of understanding, e.g. contract address, which is called by one name in all tables. For example, with the suffix `daily_stats`,  the table  name speaks for itself - table is updated daily. Another example `info` suffix - always consists static data.
3. **Optimise the index**. This is necessary to ensure that the table can be quickly queried
4. **Not to repeat the information**. Repeating information across multiple tables can lead to inconsistency and errors.
5. **Ensure data integrity**. This is achieved by using foreign keys and other database tools.
6. **Keep the data model as simple as possible**. This is necessary to ensure that it can be easily extended and maintained.
7. **Solve the problem of unassociated data.** Provide basic information tables with `_info` suffix to association of internal and external table data.

## **Naming convention**

### **Common - tables and fields**

1. Table name and fields name are in lowercase
2. Underscores separate the distinct terms as per the standard conventions
3. All table names are in plural form&#x20;
4. Table names are only having the following characters:&#x20;
   1. a to z / A to Z
   2. 0 to 9
   3. underscore (`_`) instead of spaces&#x20;
5. Table names may have multiple underscores

### **Tables**

#### **Prefixes**

`ud_`: means user define, data contributed by the community.

#### Suffixes

`_info` : represents the base information table maintained by Footprint and can be used as a hub for data association

`_daily_stats`. Data in the table are aggregated by day.

`_token_transfers`. Flow records of data chain tokens.

`_transactions`. Represents transaction that occurs on the blockchain, and the hash value represents its uniqueness.

`_deprecated`. Table is no longer relevant.

{% hint style="info" %}
* Same `{table}` may be deprecated several times. Following popular naming convention, the deprecated tables will have the autoincrimenting number appended so that the table name will look like following: `{table}_depecated_{copy_number}`
* Deprecated tables will only be for 30 days. Users having the charts that are based on deprecated tables will be guided to use new updated tables instead
{% endhint %}

#### Special marks

`Beta`**:** data accuracy, stability, data period, update frequency and other important metrics are still being tested
