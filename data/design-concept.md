# 🏗 Design concept

Building ETL processes for blockchains involves processing huge amounts of unstructured data. Accordingly, designing a database is a non-trivial task. In the initial design of the data model, we pursued the following goals:

1. **Reduce the number table joins**. With the most frequently used combination of slug+chain, you can quickly find the data you want in multiple tables.
2. **Reduce the cost of understanding**. Consistent presentation of multiple fields in different tables, reduces the cost of understanding, e.g. contract address, which is called by one name in all tables. For example, with the suffix `daily_stats`,  the table  name speaks for itself - table is updated daily. Another example `info` suffix - always consists static data.
3. **Optimise the index**. This is necessary to ensure that the table can be quickly queried
4. **Not to repeat the information**. Repeating information across multiple tables can lead to inconsistency and errors.
5. **Ensure data integrity**. This is achieved by using foreign keys and other database tools.
6. **Keep the data model as simple as possible**. This is necessary to ensure that it can be easily extended and maintained.
7. **Solve the problem of unassociated data.** Provide basic information tables with `_info` suffix to association of internal and external table data.

With these goals in mind, we used the following approaches to organise the data:

{% hint style="info" %}
The quick answer is that we have a special approach to data organisation, as well as an architecture that uses the most relevant data science tools and approaches
{% endhint %}

**Lego**

Footprint defines a DeFi Lego hierarchy with a business logic abstraction layer, based on traditional financial instrument hierarchy and smart contract characteristics. It tags on-chain transactions with this Lego hierarchy and transforms unstructured data split out from smart contracts into structured and meaningful data. We designed the database with different business domains and different components for each domain, which can be combined like Lego - through the combination we can quickly parse on-chain data and bring it into a structure and standard data tables. Take a look at the following examples:

<figure><img src="../.gitbook/assets/Screenshot 2022-09-05 at 11.50.58 (1).png" alt=""><figcaption><p>NFT Lego hierarchy</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2022-09-05 at 11.55.24.png" alt=""><figcaption><p>Defi Lego hierarchy</p></figcaption></figure>

**Layering**

Also we have an important additional step - tiering of tables. We divide tables from different domains into bronze, silver and gold. See more in [data-structure.md](data-structure.md "mention") and [data-domains.md](data-domains.md "mention").

**Semantic categorisation**

There are different ways how the event could be called and infinite ways how it could be named.  We do not find it a good experience for analysts to go read a smart contract code to understand at what exact point the event was emitted so that it is clear what business knowledge could be extracted. No matter what the code for minting a NFT on a specific chain looks like, one needs to find a way to put all of this data into one category, called `Minting`.&#x20;

It is this organization of data that allows you to achieve the following:

#### Footprint is much faster

Whereas other popular solutions need to recompute high level indicators every time from raw event data, in Footprint with the data layers abstraction layers (silver and gold), the amount of work is significantly reduced to query key information. Ultimately, user requests are completed in milliseconds, where similar requests can take minutes on other platforms.

![Footprint abstract overview](https://static.footprint.network/card\_images/d411037b-7258-436c-b696-5bc7c10e8e13.jpg)

With the sophisticated architecture in the background come the caching mechanisms that greatly reduce redundant work and computing resource from O(n) to O(1). Dataset previously queried will be saved in cache and will be used during the next query execution. That way, users get their requests fast and our network don’t experience overloads so other users are not affected.

#### Several interfaces

The slow execution of requests completely closes access to the DBaaS model through various APIs. With the speed of query execution and the amount of data provided, we are leaders in providing and keeping data up-to-date to our partners. Check out [api](../guides/api/ "mention") for more.

It cleans and integrates on-chain data so users of any experience level can quickly start researching tokens, projects and protocols. With over a thousand dashboard templates plus a drag-and-drop interface, anyone can build their own customised charts in minutes. Uncover blockchain data and discover the value trend behind the project.
