# Ethereum Data

**ethereum\_token\_transfer**

This table shows ERC20 tokens transfer events (e.g. sender address, receiver address, token address, amount of tokens sent, etc) on Ethereum chain.

| block\_hash       | string    | a unique identifier for block                                                                               |
| ----------------- | --------- | ----------------------------------------------------------------------------------------------------------- |
| block\_number     | integer   | length of the blockchain in blocks                                                                          |
| block\_timestamp  | timestamp | time at which the transaction occurred                                                                      |
| from\_address     | string    | address of transaction sender                                                                               |
| log\_index        | integer   | transaction index                                                                                           |
| to\_address       | string    | address of transaction receiver                                                                             |
| token\_address    | string    | address of the erc20 token                                                                                  |
| transaction\_hash | string    | transaction hash                                                                                            |
| value             | numeric   | amount of erc20 tokens sent. Notice that you have divided this by the relevant decimals of the erc20 token. |
| decimals          | integer   | value divided by decimals                                                                                   |
| cal\_value        | float     | value calculated by dividing value by decimals                                                              |
| symbol            | string    | erc20 token symbol                                                                                          |
| price             | float     | erc20 token price                                                                                           |

**ethereum\_transactions**

This table shows the details of every transaction (e.g. sender address, receiver address, transaction value, gas, etc.) on Ethereum chain.

| field name                     | data type                         | field description                                                                          |
| ------------------------------ | --------------------------------- | ------------------------------------------------------------------------------------------ |
| hash                           | string                            | transaction hash                                                                           |
| nonce                          | integer                           | block nonce is used to demonstrate the proof of work during mining                         |
| transaction\_index             | integer                           | transaction index                                                                          |
| from\_address                  | string                            | address of transactions sender                                                             |
| to\_address                    | string                            | address of transaction receiver                                                            |
| value                          | float                             | value being transacted in Ether and fiat value                                             |
| gas                            | integer                           | gas of the current block                                                                   |
| gas\_price                     | integer                           | gas price of the current block                                                             |
| block\_timestamp               | timestamp                         | time at which the transaction occurred                                                     |
| block\_number                  | integer                           | length of the blockchain in blocks                                                         |
| block\_hash                    | string                            | unique identifier for that block                                                           |
| receipt\_cumulative\_gas\_used | integer                           | Total amount of gas used when this transaction was executed in the block                   |
| receipt\_gas\_used             | integer                           | Amount of gas used by this specific transaction alone                                      |
| receipt\_contract\_address     | string                            | The contract address created,  if the transaction was a contract creation, otherwise null  |
| receipt\_root                  | string                            | 32 bytes of post-transaction stateroot (pre-Byzantium)                                     |
| receipt\_status                | integer                           | Either 1 (success) or 0 (failure) (post-Byzantium)                                         |
| max\_fee\_per\_gas             | integer                           | Total fee that covers both base and priority fees                                          |
| max\_priority\_fee\_per\_gas   | integer                           | Fee given to miners to incentivize them to include the transaction                         |
| transaction\_type              | integer                           | Transaction type                                                                           |
| receipt\_effective\_gas\_price | integer                           | Actual value per gas deducted from the sender account. Replacesf gas\_price after EIP-1559 |
| base\_fee\_per\_gas            | integer                           | Base fee                                                                                   |
