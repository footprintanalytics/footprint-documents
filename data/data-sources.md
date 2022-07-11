# Sources

## Blockchain

Most data comes from different blockchains. We automatically pick up blocks, logs, traces, transactions on the blockchain.

## Off-chain

In order to provide users with more comprehensive information, Footprint aggregates some off-chain data from:

1. Community contributions (i.e. `protocol_info` table: logo, twitter, discord, etc.)
2. Aggregators, such as Coingecko’s (i.e. `token_info, token_daily_stats` tables)

## Defined by users

1. Usually, the table starts with `ud`
2. Footprint provides CSV and API upload to users to upload data to do personalized analysis.

{% hint style="danger" %}
The data uploaded by the community is not verified and it is up to the community to ensure the accuracy of the data.
{% endhint %}
