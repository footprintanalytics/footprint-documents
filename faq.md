# ❓ FAQ

<details>

<summary></summary>



</details>

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

1. No code experience, users can easily analyse the data on the chain without writing SQL
2. Cross-chain analysis supported
3. Combination of on-chain and off-chain data analysis supported
4. Ability to upload own data
5. Semantic data, and users can quickly understand the complex data on the chain.

</details>

<details>

<summary><strong>What dialect of SQL does Footprint use (e.g., postgresql, mysql, etc.)?</strong></summary>

For fast querying, we use Doris (an OLAP DB), which supports the American National Standards Institute (ANSI).

</details>

<details>

<summary><strong>How can I know the time range of each data table?</strong></summary>

You can open the[ Footprint Datasets & Data Dictionary](https://www.footprint.network/@Footprint/Footprint-Datasets-Data-Dictionary) dashboard and see the 'Time Period'and 'Table Description' for each data table. You can click on the hyperlink for each data table to see the details.

</details>

<details>

<summary><strong>Can I upload data to Footprint Analytics for analysis?</strong></summary>

Yes. Footprint Analytics supports 2 ways to upload your data and cross-analyse it with existing data.

1. Using a CSV or Excel file (see [more](https://www.footprint.network/chart/custom-upload))
2. Using API upload (see [api.md](guides/api/api.md "mention"))

</details>

<details>

<summary><strong>Do you have a log / event / function call table of each chain for now? I can’t find them on your website.</strong></summary>

We do have these data tables, but the amount of raw data is too large and not yet available to the public. If you need to use them, you can join [our Discord community](https://discord.gg/3HYaR6USM7) and contact the administrator to get access to them.

</details>

<details>

<summary><strong>Which field can we use to distinguish between ERC20 / 721 / 1155 standards? Which public chains are supported?</strong></summary>

We don't currently distinguish between ERC20 / 721 / 1155, we are already working on it.

</details>
