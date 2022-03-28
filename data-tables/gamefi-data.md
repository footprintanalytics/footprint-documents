# 🎮 GameFi Data

**gamefi\_daily\_stats**

This table can be used to analyze the daily indicators (e.g. transaction volume, transaction number, transaction user number, markert cap,game's basic infomation etc ) of the GameFi.

| field name     | data type | data description                                                          |
| -------------- | --------- | ------------------------------------------------------------------------- |
| day            | timestamp | statistical date                                                          |
| protocol\_id   | numeric   | protocol id                                                               |
| protocol\_name | string    | protocol name                                                             |
| logo           | string    | logo link of the protocol                                                 |
| genre          | string    | catagory of the protocol                                                  |
| is\_f2p        | string    | whether the game is free                                                  |
| is\_p2e        | string    | whether the game is profitable                                            |
| users          | integer   | number of unique wallet addresses interacting with dapp's smart contracts |
| transactions   | integer   | transactions made to dapp's smart contracts                               |
| volume         | float     | total amount of incoming value to dapp's smart contracts                  |
| balance        | float     | total value of assets in dapp's smart contract                            |
