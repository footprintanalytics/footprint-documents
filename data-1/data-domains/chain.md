---
description: >-
  Footprint Database automatically synchronizes the data of the nodes on the
  chain,including every aspect of every transaction, and parses into different
  tables according to the issue to be solved.
---

# Chain

Footprint have parsed 17 chains, including&#x20;

15 EVM compatible chains: **Arbitrum, Avalanche,Boba,BSC(Binance Smart Chain),Celo,DFK(DeFi Kingdoms),Ethereum,Fantom,Harmony,HSC,Iotex,Moonbeam,Moonriver,Polygon,Thundercore**&#x20;

2 Non-EVM compatible chains: **Hive,Solana**

### **Tables for a chain**

| data level | table name                    | data contents                                                                                                                     | data dictionary                                                                                                              |
| ---------- | ----------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| **silver** | **{chain}\_transactions**     | the details of every transaction (e.g. sender address, receiver address, transaction value, gas, etc)                             | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=ethereum\_transactions)     |
| **silver** | **{chain}\_token\_transfers** | the token transfer detail of every transaction (e.g. sender address, receiver address, token address, amount of tokens sent, etc) | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=ethereum\_token\_transfers) |
| **silver** | **{chain}\_logs**             | all logs generated by smart contracts                                                                                             | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=ethereum\_logs)             |

{% hint style="info" %}
\*Check the data dictionary to get more information(field, field type,**methodology**,description)&#x20;

\***{chain}\_logs**: **** Footprint has filtered and formatted the raw bronze data, so {chain}\_logs is a silver data table.
{% endhint %}



### Known Issue&#x20;

1. The Unique Key of above 3 tables is **block\_hash.** When you need to combine data from different tables, you can use **block\_hash** to join data.&#x20;
2. **{chain}\_logs** is useful for querying protocol contracts,but it’s coded, so we need an ABI key to decode it.

### **How do communities use those tables?**

1. Monitor token liquidity: [Liquidity Monitoring - STETH ](https://www.footprint.network/@Momo/Liquidity-Monitoring-stETH)
2. Monitor token mint and burn:[ETH Burned](https://www.footprint.network/guest/dashboard/0663e0a7-2ed7-430e-abf9-eea60edda373)&#x20;
3. Monitor pool of protocol,including liquidity, whales:[Curve Dashboard ](https://www.footprint.network/guest/dashboard/9f4d30ce-9676-43a9-bf31-2712632b4bf1)
4. Analyze Gas fee: [Gas Dashboard](https://www.footprint.network/@DamonSalvatore/Gas-Dashboard?date=past3months\~)




