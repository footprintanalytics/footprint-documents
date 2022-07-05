# DeFi

### **Tables for DeFi**

| data leve  | table name                             | data contents                                                                                                                              | data dictionary                                                                                                                      |
| ---------- | -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| **silver** | **protocol\_info**                     | <p>protocol basic info</p><p>(including token symbol, logo,token address,etc)</p>                                                          | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_info)                     |
| **silver** | **defi\_pool\_info**                   | <p>DeFi pool basic info</p><p>(including chain, protocol slug,pool name,deposit contract address, return token,etc)</p>                    | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_pool\_info)                   |
| **silver** | **defi\_pool\_info\_return\_token**    | Return token for each DeFi pool                                                                                                            | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_pool\_info\_return\_token)    |
| **silver** | **defi\_transactions\_90d**            | <p>the DeFi protocols transaction details</p><p>(including chain, contract address, operator,pool,token,transaction value,etc)</p>         | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_transactions\_90d)            |
| **gold**   | **defi\_protocol\_daily\_stats**       | the protocol daily indicators (including protocol slug,TVL, volume,etc )                                                                   | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_protocol\_daily\_stats)       |
| **gold**   | **dex\_pool\_liquidity\_daily\_stats** | the add/remove liquidity transaction of DeFi Dexes (including pool name, add/remove liquidity,transaction amount, etc)                     | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=dex\_pool\_liquidity\_daily\_stats) |
| **gold**   | **dex\_pool\_swap\_daily\_stats**      | <p>the swap transactions of DeFi Dexes</p><p>(including pool name, send/receive token,transaction amount,volume, etc)</p>                  | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=dex\_pool\_swap\_daily\_stats)      |
| **gold**   | **lending\_pool\_daily\_stats**        | <p>the transactions of DeFi Lending protocols</p><p>(including pool name,deposit/collateral/borrow token &#x26; amount, flashloan,etc)</p> | [**data dictionary>**](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=lending\_pool\_daily\_stats)        |

{% hint style="info" %}
Click the table name to check the data dictionary to get more information(field, field type,**methodology**,description)
{% endhint %}

### Known issue

The unique keys for joining datasets are **protocol\_slug/pool\_name.**

### How do communities use those tables?

1. Monitor DeFi stats of chain
   1. [Chain Overview](https://www.footprint.network/guest/dashboard/35dfdf0f-5c59-4504-9907-7374eae92981?date\_filter=past90days)
   2. [Solana Analysis Dashboard](https://www.footprint.network/guest/dashboard/e22e8f10-57e5-4ce8-bb34-aa8d1c65bbe1?date\_filter=2021-02-28\~)
   3. [Avalanche Dashboard](https://www.footprint.network/guest/dashboard/96093ae3-60a9-4fef-a4d3-6cb27c239f78?date=past360days)
2. Compare with different chains/ protocols: [DeFi Comparison Dashboard](https://www.footprint.network/guest/dashboard/f9786627-920e-4a57-9097-3ee2ca502736?time=past30days\&token1=aave\&token2=sushiswap)
3. Monitor Dexes Liquidity and Swap
   1. [DEX Distribution](https://www.footprint.network/guest/dashboard/cfae1cb0-2809-40cc-b5af-2ec16cadabd0)
   2. [Curve Pools](https://www.footprint.network/guest/dashboard/a955803b-adbc-45ab-baee-61b233319f2c?date=past60days\&project=Curve)
   3. [Liquidity Change VS ETH Price](https://www.footprint.network/guest/dashboard/f15a0434-3481-46c0-96ef-a311ae2dde14)
4. Monitor Lending protocols and liquidations
   1. [Lending Analysis Dashboard](https://www.footprint.network/guest/dashboard/fcc3f337-d039-4e8b-8524-71e767e77082?date=past90days\&protocol\_slug=aave\&symbol=aave)
   2. [Aave VS Compound Dashboar](https://www.footprint.network/guest/dashboard/9819c526-4bc6-4b58-9f30-70ee2401994a)d
   3. [MakerDAO Dashboard](https://www.footprint.network/guest/dashboard/6f1c3dfc-2a95-41a6-aca5-d621340de540?date\_filter=past6months\~)
   4. [Liquidation Dashboard: ETH](https://www.footprint.network/guest/dashboard/8c1242d1-e677-424f-b11d-1796decb9986?date\_filter=past60days)
   5. [Liquidation Dashboard: BTC](https://www.footprint.network/guest/dashboard/6f6d6f35-6173-479b-85d6-7b998c3ed06e?date\_filter=past30days)
5. Monitor token
   1. [StETH Dashboard](https://www.footprint.network/guest/dashboard/ccf6f47f-c1a5-46cf-8bba-caabb89287be?token\_symbol=steth\&date=past90days)
   2. [ETH\_stETH-on-Curve-Uniswap](https://www.footprint.network/guest/dashboard/0a008f14-b6cf-44d4-9b0e-47b96a0dd9b9)

***

***
