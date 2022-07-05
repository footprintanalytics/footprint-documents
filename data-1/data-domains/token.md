# Token

Footprint has included 100 k+ tokens in 110+ chains. Token price, tokenomic,holders,market cap,etc are available to analyze.

### Tables for token

| data level | table name                                                                                                                         | data contents                                                                                                                                                  |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| silver     | [token\_info](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_info)                               | <p>token basic info</p><p>(including token symbol, logo,token address,etc)</p>                                                                                 |
| gold       | [token\_chain\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_chain\_daily\_stats) | <p>the token daily indicators on multiple chains</p><p>(including tokenomic,mint and burn amount, number of active address/ new address/ transactions,etc)</p> |
| gold       | [token\_daily\_stats](https://www.footprint.network/@Footprint/Table-Info-Dashboard?table\_name=token\_daily\_stats)               | the token daily indicators (including token price,market cap,trade volume, FDV,supply,etc )                                                                    |

{% hint style="info" %}
Click the table name to check the data dictionary to get more information(field, field type,**methodology**,description)
{% endhint %}

### Known issue

The unique key for joining datasets is **token\_slug.**

### How do communities use those tables?

1. Monitor tokenomic of token:
   1. holders/mint/burn:[Tokenomics of (Token)](https://www.footprint.network/guest/dashboard/aa971726-d7a8-4963-8001-a83a4222741e?token\_address=0x26193c7fa4354ae49ec53ea2cebc513dc39a10aa)
   2. token Issuance;token users & transactions:[Tokenomic V2.0](https://www.footprint.network/guest/dashboard/3e0d4c65-ac84-4cea-a5d0-a2b1aa67f04d?token\_name=hashland-coin)
   3. [Token Volume](https://www.footprint.network/guest/dashboard/652af0c2-083b-43a2-83d8-fa2cbb61ab1e?date\_range=2021-10-01\~2021-10-31\&symbol=luna)
2. Monitor token price: [UST & LUNA Death Spiral Analysis](https://www.footprint.network/guest/dashboard/6a8a2d49-ea37-41bf-b5df-8c028ed97bc2?back\_url=https%3A%2F%2Fwww.footprint.network%2F%40Footprint%2FTable-Info-Dashboard%3Ftable\_name%3Dtoken\_chain\_daily\_stats)
3. Monitor token of protocol:
   1. [DeFi Kingdoms - CRASTAL](https://www.footprint.network/guest/dashboard/729e9417-199e-44dc-961f-e8b72df957d0?gamefi\_name=defi-kingdoms\&chain=DFK\&token=DeFi%20Kingdoms%20Crystal)
   2. [StepN Token Daily Stats Dashboard](https://www.footprint.network/guest/dashboard/9d4750e5-90ba-4f97-a661-b46219bc5dd5?series\_date=past90days)
