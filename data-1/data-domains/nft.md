# NFT

Footprint has included 6000+ NFT collections, and indexed the data of following marketplaces:

1. Opensea
2. LooksRare
3. X2Y2

### Tables for NFT

| data leve | table name                    | data contents                                                                                                                  | data dictionary                                                                                                            |
| --------- | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| silver    | nft\_collection\_info         | <p>NFT collection basic info</p><p>(including chain, contract address,protocol slug,etc)</p>                                   | [data dictionary](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_collection\_info)         |
| silver    | nft\_transactions             | the NFT transaction details (including chain, contract address, from/to address,marketplace,transaction value,etc)             | [data dictionary](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_transactions)             |
| gold      | nft\_latest\_stats            | <p>the NFT latest data</p><p>(including latest price, current hold time,laest owner, past owners,etc )</p>                     | [data dictionary](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_latest\_stats)            |
| gold      | nft\_collection\_daily\_stats | the NFT collections daily indicators (including price,liquidity,volume,number of buyers/sellers/holders,mint,transactions,etc) | [data dictionary](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=nft\_collection\_daily\_stats) |

{% hint style="info" %}
Check the data dictionary to get more information(field, field type,**methodology**,description)
{% endhint %}

### Known issue

The unique keys for joining datasets are **protocol\_slug /collection\_name**.

### How do communities use those tables?

1. Monitor NFT collection
   1. [Meebits Data Analysis](https://www.footprint.network/guest/dashboard/306f993b-8ce3-4710-9ca7-e678110215b3?series\_date=past90days)
   2. [Hashland NFT Dashboard](https://www.footprint.network/guest/dashboard/797c63e0-1bf3-4dfc-af80-1eee5dabad3d)
2. Monitor NFT stats of Chain:[NFT Market Overview on Ethereum](https://www.footprint.network/guest/dashboard/9189d1a0-b0e2-4b65-b45d-d01ef2b83bf4?series\_date=past90days)
3. Monitor NFT stats of GameFi:[NFT Collection Stats of GameFi](https://www.footprint.network/guest/dashboard/22c585eb-9d28-4211-8310-c00db76b933e?nft\_collection=starsharks)
