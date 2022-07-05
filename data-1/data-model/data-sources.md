# Data sources

Sources of Footprint Data:

### Blockchain

1. Most data comes from blockchains. Our Database automatically picks up blocks, logs, traces,transactions on the blockchain.
2. Those raw bronze data are transformed into user-usable silver and gold data.

### Off-chain

In order to provide users with more comprehensive information, Footprint aggregates some off-chain data：

1.  Generally community contributions

    protocol\_info:logo, twitter,discord,etc
2.  Aggregates Coingecko’s token data,coming from open API

    token\_info

    token\_daily\_stats

### User Define

1. Usually, the table starts with”ud”(User Define)
2. Footprint provides CSV and API upload to users to upload data to do personalized analysis.
3. **The data uploaded by the community is not verified and it is up to the community to ensure the accuracy of the data.**
