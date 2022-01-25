# DEX Data

#### dex\_pair\_daily\_stats&#x20;

This table shows the transaction pair information (e.g. volume, number of transactions, tokens price, etc.) of DEX platforms on different chains.

| field name       | data type | field description                                       |
| ---------------- | --------- | ------------------------------------------------------- |
| protocol\_id     | numeric   | protocol id                                             |
| protocol\_slug   | string    | abbreviation of the protocol                            |
| name             | string    | protocol name                                           |
| chain            | string    | chain of the protocol                                   |
| volume           | float     | trading volume in USD of this protocol in last 24 hours |
| token\_0         | string    | first token address in the trading pair                 |
| token\_0\_symbol | string    | first token symbol in the trading pair                  |
| token\_0\_price  | float     | first token value(USD) in the trading pair              |
| token\_1         | string    | second token address in the trading pair                |
| token\_symbol    | string    | second token symbol in the trading pair                 |
| token\_1\_price  | float     | second token value(USD) in the trading pair             |
| day              | timestamp | statistical date                                        |
| trade\_count     | integer   | transaction number of the Dex pair                      |
| annualized\_fee  | float     | annualized fee per transaction pair                     |
| total\_liquidity | float     | cumulative liquidity of trading pairs                   |
| fee\_24h\_quote  | float     | 24-hour transaction fee for trading pairs               |

#### dex\_daily\_stats&#x20;

This table can be used to analyze the daily indicators (e.g.volume, number of transactions, etc.) of different DEXplatforms on different chains.

| field name                 |    date type        | field description                                      |
| -------------------------- | ------------------- | ------------------------------------------------------ |
| day                        | tiemstamp           | the statistical date                                   |
| protocol\_id               | numeric             | protocol id                                            |
| name                       | string              | protocol name                                          |
| protocol\_slug             | string              | abbreviation of the protocol                           |
| chain                      | string              | chain of the protocol                                  |
| volume                     | float               | trading volume in USD of protocol in the last 24 hours |
| trade\_count               | integer             | transaction number of the Dex pair                     |
