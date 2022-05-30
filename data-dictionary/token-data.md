# 🪙 Token Data

#### token

This table allows you to easily find basic information about ERC20 tokens on the Ethereum chain.

| coin\_id      | string    | unique id             |
| ------------- | --------- | --------------------- |
| symbol        | string    | identifier of token   |
| token         | string    | address of token      |
| total\_supply | float     | total supply of token |
| created\_at   | timestamp | time of data created  |
| updated\_at   | timestamp | time of  data updated |

#### token\_daily\_stats  &#x20;

This table can be used to analyze the daily indicators (e.g. price, total value locked, trade volume in 24 hours, current market capitalization, etc ) of the ERC20 token on Ethereum chain.

| field name                                      | data type                           | field description                                                               |
| ----------------------------------------------- | ----------------------------------- | ------------------------------------------------------------------------------- |
| address                                         | string                              | address of the token                                                            |
| symbol                                          | string                              | identifier of the token                                                         |
| category                                        | string                              | platform type ot the protocol                                                   |
| price                                           | float                               | price of the end of day                                                         |
| day                                             | timestamp                           | statistical date                                                                |
| market\_cap                                     | float                               | total market value of a cryptocurrency’s circulating supply                     |
| fully\_diluted\_valuation                       | float                               | total market value of after cryptocurrency fully diluted                        |
| total\_supply                                   | float                               | amount of coins traded , minus any coins that have been burned                  |
| max\_supply                                     | float                               | maximum number of coins coded to exist in the lifetime of the cryptocurrency    |
| circulating\_supply                             | float                               | amount of coins that are circulating in the market and tradeable by the public  |
| market\_cap\_rank                               | float                               | rank of market capitalization                                                   |
| low\_price\_24h                                 | float                               | lowest price in last 24 hours                                                   |
| high\_price\_24h                                | float                               | highest price in last 24 hours                                                  |
| trading\_vol\_24h                               | float                               | cryptocurrency trading volume across all tracked platforms in the last 24 hours |
| coin\_id                                        | string                              | unique id of coin id                                                            |



