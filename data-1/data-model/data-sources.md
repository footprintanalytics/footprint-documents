# Data Sources

Sources of Footprint Data:

### Blockchain&#x20;

1. Most data comes from blockchains. Our Database automatically picks up blocks, logs, traces,transactions on the blockchain.&#x20;
2. Those raw bronze data are transformed into user-usable silver and gold data.&#x20;

### Off-chain&#x20;

In order to provide users with more comprehensive information, Footprint aggregates some off-chain data：&#x20;

1. Generally community contributions
   1. protocol\_info:logo, twitter,discord,etc&#x20;
2. Aggregates Coingecko’s token data,coming from open API
   1. token\_info&#x20;
   2. token\_daily\_stats&#x20;

### User Define&#x20;

1. Usually, the table starts with”ud”(User Define)&#x20;
2. Footprint provides CSV and API upload to users to upload data to do personalized analysis.&#x20;
3. **The data uploaded by the community is not verified and it is up to the community to ensure the accuracy of the data.**
