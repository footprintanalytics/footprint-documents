# 🎭 Social Data

**socialfi\_daily\_stats**

This table can be used to analyze the daily indicators (e.g. transaction volume, transaction number, transaction user number, markert cap, etc ) of the GameFi.

| field name     | data type | field description                                                         |
| -------------- | --------- | ------------------------------------------------------------------------- |
| day            | timestamp | statistical date                                                          |
| protocol\_id   | numeric   | protocol id                                                               |
| protocol\_name | string    | protocol name                                                             |
| protocol\_slug | string    | abbreviation of the protocol                                              |
| logo           | string    | the logo link of the protocol                                             |
| chain          | string    | the chain of the protocol                                                 |
| transactions   | integer   | transactions made to dapp's smart contracts                               |
| users          | integer   | number of unique wallet addresses interacting with dapp's smart contracts |
| volume         | float     | total amount of incoming value to dapp's smart contracts                  |
| balance        | float     | total value of assets in dapp's smart contract                            |
