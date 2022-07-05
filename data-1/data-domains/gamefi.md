# GameFi

### **Tables for GameFi**

| data level | table name                                                                                                                                 | data contents                                                                                                                   |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| gold       | [gamefi\_protocol\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=gamefi\_protocol\_daily\_stats) | <p>GameFi daily indicators</p><p>(including chain,protocol slug, game genre, number of transactions/users, TVL,volume,etc )</p> |
| silver     | [protocol\_info](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_info)                                 | protocol basic info (including token symbol, logo,token address,etc)                                                            |
| silver     | [protocol\_transactions](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_transactions)                 | the protocols transaction details (including chain, contract address, method,transaction value,etc)                             |
| gold       | [protocol\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_daily\_stats)                 | the protocol daily active/new address (including number of active address/ new address,unique address,etc )                     |
| gold       | [protocol\_active\_address](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_active\_address)           | the protocol daily active address (including DeFi,NFT,GameFi protocols)                                                         |
| silver     | [nft\_collection\_info](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_collection\_info)                   | <p>NFT collection basic info</p><p>(including chain, contract address,protocol slug,etc)</p>                                    |
| silver     | [nft\_transactions](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_transactions)                           | the NFT transaction details (including chain, contract address, from/to address,marketplace,transaction value,etc)              |
| gold       | [nft\_latest\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_latest\_stats)                         | <p>the NFT latest data</p><p>(including latest price, current hold time,laest owner, past owners,etc )</p>                      |
| gold       | [nft\_collection\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_collection\_daily\_stats)   | the NFT collections daily indicators (including price,liquidity,volume,number of buyers/sellers/holders,mint,transactions,etc)  |

{% hint style="info" %}
Click the table name to check the data dictionary to get more information(field, field type,**methodology**,description)
{% endhint %}

### Known issue

The unique key for joining datasets is **protocol\_slug**.

### How do communities use those tables?

1. Monitor GameFi industry
   * [GameFi Overview](https://www.footprint.network/guest/dashboard/c358ff97-6bf6-491c-b9fd-645fb8262e3f)
   * [Dashboard For GameFi Industry](https://www.footprint.network/guest/dashboard/f7d88ee8-9341-49ae-b497-088bee7ec038?date=past60days)
2. Track Games
   * [GameFi Tracker](https://www.footprint.network/guest/dashboard/f39ac368-f265-4ae3-8466-8385e06c043d?relative\_date=past30days)
   * [Axie Infinity Dashboard](https://www.footprint.network/guest/dashboard/db8d941f-2a74-4120-abd4-ff20fc032a5e)
