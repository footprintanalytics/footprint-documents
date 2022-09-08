# ❓ FAQ

<details>

<summary><strong>Are there any documents about the data source?</strong></summary>

There are 3 data sources:

1. On-chain data (DeFi, NFTs, GameFi and etc.)
2. Off-chain data (i.e some token prices come from the Coingecko API)
3. Data uploaded by community

</details>

<details>

<summary><strong>My project just launched, how do I get the parsed data on Footprint?</strong></summary>

If your project is on one of our launched chains, you can submit your contract address to us for parsing via [https://www.notion.so/Contract-Addresses-7989b1592ad24011a508ce3db601bb32](https://www.notion.so/Contract-Addresses-7989b1592ad24011a508ce3db601bb32)

</details>

<details>

<summary><strong>What's the difference between competitors and Footprint Analytics?</strong></summary>

* No code experience, users can easily analyse the data on the chain without writing SQL
* Cross-chain analysis supported
* Combination of on-chain and off-chain data analysis supported
* Ability to upload own data
* Semantic data, and users can quickly understand the complex data on the chain.

</details>

<details>

<summary><strong>What dialect of SQL does Footprint use?</strong></summary>

For fast querying, we use Doris (an OLAP DB), which supports the American National Standards Institute (ANSI).

</details>

<details>

<summary><strong>How can I know the time range of each data table?</strong></summary>

You can open the[ Footprint Datasets & Data Dictionary](https://www.footprint.network/@Footprint/Footprint-Datasets-Data-Dictionary) dashboard and see the `Time period` and `Table Description` for each data table. You can click on the hyperlink for each data table to see the details.

</details>

<details>

<summary><strong>Can I upload data to Footprint Analytics for analysis?</strong></summary>

Yes. Footprint Analytics supports 2 ways to upload your data and cross-analyse it with existing data.

1. Using a CSV or Excel file (see [more](https://www.footprint.network/chart/custom-upload))
2. Using API upload (see [api.md](../guides/api/api.md "mention"))

</details>

<details>

<summary><strong>Do you have a log / event / function call table of each chain for now? I can’t find them on your website.</strong></summary>

We do have these data tables, but the amount of raw data is too large and not yet available to the public. If you need to use them, you can join [our Discord community](https://discord.gg/3HYaR6USM7) and contact the administrator to get access to them.

</details>

<details>

<summary>How do we monitor the addition of new contracts?</summary>

Getting new contract addresses from external sources was our early practice, and we have now iterated to an automated solution that identifies contract addresses from our own foundation tables (`transactions`, `token_transfers` and etc.). When incremental node data is found to contain contract addresses that are not included in the database yet, the mechanism will automatically collect them.

</details>

<details>

<summary><strong>What do you mean by NFT aggregators? How can you define volume from different marketplaces?</strong></summary>

An NFT marketplace aggregator consolidates the listing inventory of multiple different marketplaces, allowing users to gain full transparency of the market and also buy and sell NFTs in bulk without having to interact with each separate marketplace. We regard NFT aggregators as a marketplace from the event parsing process.&#x20;

Aggregators transactions will not only have the marketplace name, but the aggregator name will be included too. In special cases( such as more than 2 aggregators are involved) we will just display the name of the first aggregator trigger the trade.

</details>

<details>

<summary><strong>Why do users use the API and not use the Footprint front-end directly?</strong></summary>

Footprint's front-end UI is very powerful in terms of analytics and can meet most data analysis and visualization needs. The API service is mainly for enterprise level customers, who have higher requirements for data, data analysis or simply want to use the programming interface to integrate the data from Footprint to the applications.

</details>

<details>

<summary>How do we verify the quality of data?</summary>

There are several strategies that we use to validate data:

**Basic validation**

No unusual data is present. Different traditional statistical methods are used for verification. No gaps in time between data are present.

**Logical (internal) validation**

The data makes sense in terms of business metrics. For instance, most lending protocols usually require overcollateralization. Therefore the net deposit amount should be higher than net borrowing amount.

**Cross-validation**

Finally we compare the calculated metrics like TVL and MC with other data platforms

</details>
