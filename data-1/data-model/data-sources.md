# Data sources

## Blockchain

1. Most data comes from blockchains. Our Database automatically picks up blocks, logs, traces,transactions on the blockchain.
2. Those raw bronze data are transformed into user-usable silver and gold data.

## Off-chain

In order to provide users with more comprehensive information, Footprint aggregates some off-chain data：

1.  Generally community contributions

    `protocol_info`:logo, twitter,discord,etc
2.  Aggregates Coingecko’s token data,coming from open API

    `token_info,token_daily_stats`

## Defined by users

1. Usually, the table starts with `ud`
2. Footprint provides CSV and API upload to users to upload data to do personalized analysis.

{% hint style="danger" %}
The data uploaded by the community is not verified and it is up to the community to ensure the accuracy of the data.
{% endhint %}
