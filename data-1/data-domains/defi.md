# DeFi

### **Tables for DeFi**

| data level | table name                                                                                                                                         | data contents                                                                                                                                                  |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| silver     | ``[`defi_pool_info`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_pool\_info)``                                 | <p>DeFi pool basic info</p><p>(including chain, protocol slug,pool name,deposit contract address, return token,etc)</p>                                        |
| silver     | [`defi_transactions_90d`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_transactions\_90d)``                     | <p>the DeFi protocols transaction details</p><p>(including chain, contract address, operator,pool,token,transaction value,etc)</p>                             |
| gold       | [`defi_protocol_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=defi\_protocol\_daily\_stats)``            | the protocol daily indicators (including protocol slug,TVL, volume,etc )                                                                                       |
| gold       | [`dex_pool_liquidity_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=dex\_pool\_liquidity\_daily\_stats)`` | the add/remove liquidity transaction of DeFi Dexes (including pool name, add/remove liquidity,transaction amount, etc)                                         |
| gold       | ``[`dex_pool_swap_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=dex\_pool\_swap\_daily\_stats)``         | <p>the swap transactions of DeFi Dexes</p><p>(including pool name, send/receive token,transaction amount,volume, etc)</p>                                      |
| gold       | [`lending_pool_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=lending\_pool\_daily\_stats)``              | <p>the transactions of DeFi Lending protocols</p><p>(including pool name,deposit/collateral/borrow token &#x26; amount, flashloan,etc)</p>                     |
| silver     | ``[`protocol_info`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_info)``                                    | protocol basic info (including token symbol, logo,token address,etc)                                                                                           |
| silver     | [`protocol_transactions`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_transactions)``                      | <p>the protocols transaction details</p><p>(including chain, contract address, method,transaction value,etc)</p>                                               |
| gold       | [`protocol_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_daily\_stats)``                       | <p>the protocol daily active/new address</p><p>(including number of active address/ new address,unique address,etc )</p>                                       |
| gold       | ``[`protocol_active_address`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_active\_address)``               | the protocol daily active address (including DeFi,NFT,GameFi protocols)                                                                                        |
| silver     | ``[`token_info`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_info)``                                          | <p>token basic info</p><p>(including token symbol, logo,token address,etc)</p>                                                                                 |
| gold       | [`token_chain_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_chain\_daily\_stats)``                | <p>the token daily indicators on multiple chains</p><p>(including tokenomic,mint and burn amount, number of active address/ new address/ transactions,etc)</p> |
| gold       | [`token_daily_stats`](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_daily\_stats)``                             | the token daily indicators (including token price,market cap,trade volume, FDV,supply,etc )                                                                    |

{% hint style="info" %}
Click the table name to check the data dictionary to get more information(field, field type, **methodology**, description)
{% endhint %}

### Known issue

The unique keys for joining datasets are `protocol_slug`/`pool_name`.

### How do communities use those tables?

1. Monitor DeFi stats of chain
   * [Chain Overview](https://www.footprint.network/guest/dashboard/35dfdf0f-5c59-4504-9907-7374eae92981?date\_filter=past90days)
   * [Solana Analysis Dashboard](https://www.footprint.network/guest/dashboard/e22e8f10-57e5-4ce8-bb34-aa8d1c65bbe1?date\_filter=2021-02-28\~)
   * [Avalanche Dashboard](https://www.footprint.network/guest/dashboard/96093ae3-60a9-4fef-a4d3-6cb27c239f78?date=past360days)
2. Compare with different chains/ protocols: [DeFi Comparison Dashboard](https://www.footprint.network/guest/dashboard/f9786627-920e-4a57-9097-3ee2ca502736?time=past30days\&token1=aave\&token2=sushiswap)
3. Monitor Dexes Liquidity and Swap
   * [DEX Distribution](https://www.footprint.network/guest/dashboard/cfae1cb0-2809-40cc-b5af-2ec16cadabd0)
   * [Curve Pools](https://www.footprint.network/guest/dashboard/a955803b-adbc-45ab-baee-61b233319f2c?date=past60days\&project=Curve)
   * [Liquidity Change VS ETH Price](https://www.footprint.network/guest/dashboard/f15a0434-3481-46c0-96ef-a311ae2dde14)
4. Monitor Lending protocols and liquidations
   * [Lending Analysis Dashboard](https://www.footprint.network/guest/dashboard/fcc3f337-d039-4e8b-8524-71e767e77082?date=past90days\&protocol\_slug=aave\&symbol=aave)
   * [Aave VS Compound Dashboard](https://www.footprint.network/guest/dashboard/9819c526-4bc6-4b58-9f30-70ee2401994a)
   * [MakerDAO Dashboard](https://www.footprint.network/guest/dashboard/6f1c3dfc-2a95-41a6-aca5-d621340de540?date\_filter=past6months\~)
   * [Liquidation Dashboard: ETH](https://www.footprint.network/guest/dashboard/8c1242d1-e677-424f-b11d-1796decb9986?date\_filter=past60days)
   * [Liquidation Dashboard: BTC](https://www.footprint.network/guest/dashboard/6f6d6f35-6173-479b-85d6-7b998c3ed06e?date\_filter=past30days)
5. Monitor token
   * [StETH Dashboard](https://www.footprint.network/guest/dashboard/ccf6f47f-c1a5-46cf-8bba-caabb89287be?token\_symbol=steth\&date=past90days)
   * [ETH\_stETH-on-Curve-Uniswap](https://www.footprint.network/guest/dashboard/0a008f14-b6cf-44d4-9b0e-47b96a0dd9b9)

***

***
