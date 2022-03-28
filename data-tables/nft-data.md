# 🖼 NFT Data

**nft\_daily\_stats**

This table can be used to analyze the daily indicators (e.g. transaction volume, transaction number, transaction user number, markert cap, etc ) of the NFT on every chains.

| field name             | data type | data description                                    |
| ---------------------- | --------- | --------------------------------------------------- |
| day                    | timestamp | statistical date                                    |
| protocol\_id           | numeric   | protocol id                                         |
| protocol\_name         | string    | protocol name                                       |
| protocol\_slug         | string    | abbreviation of the protocol                        |
| logo                   | string    | logo link of the protocol                           |
| chain                  | string    | chain of the protocol                               |
| trading\_volume\_usd   | float     | nft trading volume with the unit of USD             |
| trading\_token\_symbol | string    | symbol of the trading token                         |
| trading\_token\_volume | string    | nft tranding volume in Token                        |
| trade\_count           | integer   | transaction numbers of the nft trading              |
| unique\_trader\_count  | integer   | number of de-duplicated nft transaction users       |
| unique\_buyers\_count  | integer   | number of de-duplicated nft transaction buyer users |
| market\_cap            | float     | total market value of the NFT circulating supply    |
