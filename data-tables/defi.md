# 🔀 DeFi

#### defi\_protocol\_info

This table covers various types of DeFi platform information on different chains.

| field name     | data type | field description                     |
| -------------- | --------- | ------------------------------------- |
| protocol\_id   | numeric   | protocol id                           |
| chain          | string    | chain of the protocol                 |
| protocol\_slug | string    | abbreviation of the protocol          |
| name           | string    | protocol name                         |
| token          | string    | token address of the protocol         |
| category       | string    | platform type ot the protocol         |
| symbol         | string    | symbol of the protocol                |
| url            | string    | link of the platform                  |
| description    | string    | description of the protocol           |
| twitter        | string    | link of Twitter account               |
| logo           | string    | logo link of the protocol             |
| coin\_id       | string    | protocol unique id                    |
| cmc\_id        | string    | protocol unique id of coin market cap |
| discord        | string    | discord link of the protocol          |
| telegram       | string    | telegram link of the protocol         |
| listed\_at     | timestamp | platform online time                  |

**defi\_daily\_stats**  &#x20;

This table can be used to analyze daily indicators (e.g.TVL, volume, etc.) of different DeFi platforms.

| protocol\_id   | numeric   | protocol id                                                                                  |
| -------------- | --------- | -------------------------------------------------------------------------------------------- |
| chain          | string    | chain of the protocol                                                                        |
| protocol\_slug | string    | abbreviation of the protocol                                                                 |
| name           | string    | protocol name                                                                                |
| tvl            | float     | capital deposited into the platform in the form of loan collateral or liquidity trading pool |
| day            | timestamp | statistical date                                                                             |

#### defi\_fundraising\_stats

This table allows you to easily find fundraising situation about the DeFi projects.

| field name          | data type | field description                             |
| ------------------- | --------- | --------------------------------------------- |
| day                 | timestamp | statistical date                              |
| id                  | string    | fundraising id                                |
| unique              | `string`  | fundraising unique id                         |
| project             | string    | fundraising project                           |
| protocol\_slug      | string    | abbreviation of the fundraising project       |
| category            | string    | category of fundraising project               |
| sub\_category       | string    | sub\_category of fundraising project          |
| website             | string    | fundraising project website url               |
| founder             | string    | founder of fundraising project                |
| fundraising\_rounds | string    | fundraising round (include project and round) |
| round               | string    | fundraising round                             |
| amount              | float     | fundraising amount                            |
| investor            | string    | investor                                      |
| description         | string    | description of fundraising project            |
| announcement        | string    | announcement of fundraising                   |
| created\_at         | timestamp | time of the data created                      |
| updated\_at         | timestamp | time of the data updated                      |

****

**organization\_daily\_info**

This table can be used to analyze daily indicators (e.g.Dao organization total revenue, total expenses,Dao members, Dao proposals, Dao voters, etc.) of the Dao organization.

| field name            | data type | field description                               |
| --------------------- | --------- | ----------------------------------------------- |
| day                   | timestamp | statistical date                                |
| organization\_id      | numeric   | Dao organization id                             |
| organization\_name    | string    | Dao organization name                           |
| platform              | string    | voting platforms that Dao organizations rely on |
| logo                  | string    | logo url of the Dao organization                |
| total\_in\_usd        | float     | Dao organization total revenue (in USD)         |
| total\_out\_usd       | float     | Dao organization total expenses (in USD)        |
| total\_value\_usd     | float     | Dao organizational total Net (in USD)           |
| total\_num\_members   | float     | total number of members of Dao organization     |
| total\_num\_proposals | float     | total number of proposals from Dao organization |
| total\_num\_voters    | float     | total number of votes in Dao organization       |
| voters\_participation | float     | Dao organization voting rate                    |

****

**organization\_token\_daily\_info**&#x20;

This table allows you to easily find basic information about Dao organization tokens.

| field name              | data type | field description                                                          |
| ----------------------- | --------- | -------------------------------------------------------------------------- |
| day                     | timestamp | statistical date                                                           |
| token\_id               | numeric   | token id                                                                   |
| token\_name             | string    | token\_name                                                                |
| token\_symbol           | string    | identifier of the token                                                    |
| daos\_total\_balance    | float     | total number of tokens with that token as the dao governance token         |
| daos\_total\_usd\_value | float     | total amount of tokens with that token as the dao governance token(in USD) |
| num\_daos               | integer   | number of Dao with that token as the dao governance token                  |



**layer2\_protocol\_daily\_info**

This table covers various types of DeFi platform information on Layer2.

| field name     | data type     | dield description                           |
| -------------- | ------------- | ------------------------------------------- |
| day            | **timestamp** | statistical date                            |
| protocol\_id   | numeric       | protocol id                                 |
| protocol\_name | string        | protocol name                               |
| protocol\_slug | string        | abbreviation of the protocol                |
| logo           | string        | logo link of the protocol                   |
| purpose        | string        | purpose of protocol                         |
| technology     | string        | layer2 technology used in the protocol      |
| total\_usd     | float         | capital deposited into the protocol(in USD) |
| total\_eth     | float         | capital deposited into the protocol(in ETH) |



**layer2\_protocol\_daily\_breakdown**

This table shows the share of assets in each layer2 protocol every day.

| field name     | data type | data description                    |
| -------------- | --------- | ----------------------------------- |
| day            | timestamp | statistical date                    |
| protocol\_name | string    | protocol name                       |
| assets         | string    | asset of the protocol               |
| percentage     | numeric   | percentage of assets under protocol |



**defi\_token\_growth**

This table allows you to analyze the platform's year-over-year growth

| chain                 | string    | chain of the protocol                                                                                              |
| --------------------- | --------- | ------------------------------------------------------------------------------------------------------------------ |
| protocol\_id          | numeric   | protocol id                                                                                                        |
| name                  | string    | protocol name                                                                                                      |
| day                   | timestamp | statistical date                                                                                                   |
| logo                  | string    | logo link of the protocol                                                                                          |
| category              | string    | platform type ot the protocol                                                                                      |
| token                 | string    | token address of the protocol                                                                                      |
| protocol\_slug        | string    | abbreviation of the protocol                                                                                       |
| symbol                | string    | symbol of the protocol                                                                                             |
| tvl                   | float     | capital deposited into the platform in the form of loan collateral or liquidity trading pool                       |
| tvl\_d1\_ago          | float     | capital deposited into the platform in the form of loan collateral or liquidity trading pool on the previous day   |
| tvl\_d7\_ago          | float     | capital deposited into the platform in the form of loan collateral or liquidity trading pool on the previous week  |
| tvl\_d30\_ago         | float     | capital deposited into the platform in the form of loan collateral or liquidity trading pool on the previous month |
| price                 | float     | price of the end of day                                                                                            |
| price\_d1\_ago        | float     | price of the end of the pervious day                                                                               |
| price\_d7\_ago        | float     | price of the end of the pervious week                                                                              |
| price\_d30\_ago       | float     | price of the end of the pervious month                                                                             |
| market\_cap           | float     | total market value of a cryptocurrency’s circulating supply                                                        |
| market\_cap\_d1\_ago  | float     | total market value of a cryptocurrency’s circulating supply on the previous day                                    |
| market\_cap\_d7\_ago  | float     | total market value of a cryptocurrency’s circulating supply on the previous week                                   |
| market\_cap\_d30\_ago | float     | total market value of a cryptocurrency’s circulating supply on the previous month                                  |
| volume                | float     | cryptocurrency trading volume across all tracked platforms                                                         |
| volume\_d1\_ago       | float     | cryptocurrency trading volume across all tracked platforms on the previous day                                     |
| volume\_d7\_ago       | float     | cryptocurrency trading volume across all tracked platforms on the previous week                                    |
| volume\_d30\_ago      | float     | cryptocurrency trading volume across all tracked platforms on the previous month                                   |

