# Protocol

### Tables for Protocol

| data level | table name                                                                                                                       | data contents                                                                                                            |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| silver     | [protocol\_info](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_info)                       | <p>protocol basic info</p><p>(including token symbol, logo,token address,etc)</p>                                        |
| silver     | [protocol\_transactions](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_transactions)       | <p>the protocols transaction details</p><p>(including chain, contract address, method,transaction value,etc)</p>         |
| gold       | [protocol\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_daily\_stats)       | <p>the protocol daily active/new address</p><p>(including number of active address/ new address,unique address,etc )</p> |
| gold       | [protocol\_active\_address](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=protocol\_active\_address) | the protocol daily active address (including DeFi,NFT,GameFi protocols)                                                  |

{% hint style="info" %}
Click the table name to check the data dictionary to get more information(field, field type,**methodology**,description)
{% endhint %}

### Known issue

The unique key for joining datasets is **protocol\_slug**.

If you can't find the protocols you want to see, please submit contract address [here](https://legend-maxilla-97a.notion.site/Contract-Addresses-7989b1592ad24011a508ce3db601bb32).

### How do communities use those tables?

Monitor Protocol address(users):

1. [Address Analysis of Protocol](https://www.footprint.network/guest/dashboard/77828d1e-35bc-4b6c-90e9-7777e7c6902d?protocol\_name=decentral-games\&date\_range=past90days)
2. [BSC GameFi Tracker](https://www.footprint.network/guest/dashboard/2d160924-cc78-4c80-906d-e25b7679c843?chain=BSC\&date\_filter=past30days)
3. [GameFi User vs Token Price Analysis](https://www.footprint.network/guest/dashboard/2a4be75a-710f-49c5-8dd2-4463e29cb68c?date=past365days\~\&game\_name=My%20DeFi%20Pet\&protocol\_type=GameFi)
