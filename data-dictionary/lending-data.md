# 🔁 Lending Data

#### lending\_assets\_daily\_stats

This table can be used to analyze the indicators (e.g. asset address, deposit amount, withdrawal amount, liquidation amount, etc.) of lending platforms on different chains. Current data on this table covers only Ethereum, with more chains to be added in the future.

| field name                         | data type  | field description                                            |
| ---------------------------------- | ---------- | ------------------------------------------------------------ |
| protocol\_id                       | numeric    | protocol id                                                  |
| protocol                           | string     | protocol                                                     |
| chain                              | string     | chain of the protocol                                        |
| day                                | timestamp  | statistical date the chain of the protocol                   |
| name                               | string     | protocol  name                                               |
| protocol\_slug                     | string     | abbreviation of the protocol                                 |
| version                            | string     | platform version of the lending transaction                  |
| contract\_address                  | string     | transactions  of contract address                            |
| asset\_address                     | string     | asset address on the lending platform                        |
| asset\_symbol                      | string     | asset on the lending platform                                |
| collateral\_trade\_count           | integer    | number of platform pledge and withdrawal transactions        |
| deposit\_trade\_count              | integer    | number of platform deposit transactions                      |
| withdraw\_trade\_count             | integer    | number of platform withdraw transactions                     |
| borrow\_trade\_count               | integer    | number of borrowings on the lending platform                 |
| repay\_trade\_count                | integer    | number of platform repay transactions                        |
| deposit\_amount                    | float      | deposit amount of an asset on the lending platform           |
| deposit\__amount\_usd_             | float      | deposit amount of an asset base on usd                       |
| withdraw\_amount                   | float      | withdrawal amount of an asset on the lending platform        |
| withdraw\__amount_\_usd            | float      | withdraw amount of an asset base on usd                      |
| borrow\_amount                     | float      | borrow amount of an asset on the lending platform            |
| borrow\_amount\_usd                | float      | borrow amount of an asset base on usd                        |
| repay\_amount                      | float      | repayment amount of an asset on the lending platform         |
| repay\__amount_\_usd               | float      | repay amount of an asset base on usd                         |
| liquidation\_amount                | float      | liquidation amount of an asset on the lending platform       |
| liquidation\__amount_\_usd         | float      | liquidation amount of an asset base on usd                   |
| flashloan\_repay\_amount           | float      | amount of flash repay for an asset on the lending platform   |
| flashloan\__repay\_amount_\_usd    | float      | lashloan _repay_ amount of an asset base on usd              |
| flashloan\_borrow\_amount          | float      | amount of flash borrow for an asset on the lending platform  |
| flashloan\__borrow_\__amount\__usd | float      | lashloan _borrow_ amount of an asset base on usd             |
| outstanding                        | float      | outstanding amount of borrowing on the platform              |
| deposit\_trader\_count             | integer    | number of pledged users on the lending platform              |
| withdraw\_trader\_count            | integer    | number of withdrawal users on the lending platform           |
| borrow\_trader\_count              | integer    | number of borrow users  on the lending platform              |
| repay\_trader\_count               | integer    | number of repayment users on the lending platform            |
| liquidation\_trader\_count         | integer    | number of liquidation users                                  |
| collateral\_locked                 | float      | number of collateral                                         |
| locked\_usd\_value                 | float      | number of collateral base on usd                             |
| outstanding\_usd\_value            | float      | outstanding amount of borrowing on the platform based on usd |

