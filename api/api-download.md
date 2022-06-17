# Download Data From Footprint By Using the API
## API Models & Enum
**Chain Enum**   

| chain name  | Description | 
| ----------- | ----------- |
| Ethereum    | Ethereum chain |  




**Nft_collection_daily_stats Model** 

| Field Name |Field Type| Description | Example |
|:------------:|:-------------:|:---------------:|:---------:|
|protocol_slug|string|the protocol name of this NFT Collection|fnd|
|chain|string|the chain of this NFT Collection|Ethereum|
|contract_address|string|the contract address of this NFT Collection|0x3b3ee1931dc30c1957379fac9aba94d1c48a5405|
|on_date|string|the timestamp of this record|1654819200000|
|collection_name|string|the name of this NFT Collection|Foundation (FND)|
|number_of_mint|integer|the mint numbers of this NFT Collection up to now|0|
|number_of_transactions|integer|the total transactons of this NFT Collection up to now|45|
|number_of_burn|integer|the burn numbers of this NFT Collection up to now|0|
|number_of_sale_transactions|integer|the current sell numbers of this NFT Collection today|3|
|number_of_transfer_transactions|integer|the transfer numbers of this NFT Collection today|36|
|number_of_sellers|integer|the unique seller of this NFT Collection today|3|
|number_of_buyers|integer|the unique buyer of this NFT Collection today|1|
|number_of_holders|integer|the unique holders of this NFT Collection today|17858|
|volume|float|the current volume of this NFT Collection today|132.82993|
|market_cap|float|the marketcap of this NFT Collection on that day|3844896.8|
|total_supply|integer|the total supply of this NFT Collection up to now|132928|
|liquidity|float|the liquidity of this NFT Collection today|0.000022999999999999997|
|avg_amount|float|the avg amount of this NFT Collection today|0.026667|
|avg_price|float|the avg price of this NFT Collection today|44.276642|
|max_amount|float|the max amount of this NFT Collection today|0.03|
|min_amount|float|the min amount of this NFT Collection today|0.02|
|max_price|float|the max amount of this NFT Collection today|49.811218|
|min_price|float|the min price of this NFT Collection today|33.207481|

**Nft_collection_info Model**

| Field Name |Field Type| Description | Example |
|:------------:|:-------------:|:-------------:|:---------:|
|chain|string|the chain to which the contract belongs|Ethereum|
|protocol_slug|string|abbreviation of the protocol|-glowa-|
|contract_address|string|address of the contract|0x21e89016b10e3c46f77a86325e942e5c53813b2d|
|collection_name|string|the name of nft collection|-GLOWA-|
|logo|string|the logo of nft collection|https://lh3.googleusercontent.com/uINcT6nwbY8FPNhDZUMsoOAwfnJTKhIOJ1ii6t6ylH3lz9KWNbrfv6nD8w4VOvzmpI4mZWte1uzYjDjO5Llb3YOgzo7ERImo4M_ObZw=s120|


**Nft_latest_stats Model**

| Field Name |Field Type| Description | Example |
|:------------:|:-------------:|:-------------:|:---------:|
|chain|string|chain to which the contract belongs|Ethereum|
|contract_address|string|address of the contract|0x3b3ee1931dc30c1957379fac9aba94d1c48a5405|
|protocol_slug|string|abbreviation of the protocol|fnd|
|nft_token_id|float|id of the nft token|92544|
|longest_hold_time|integer|the longest time the nft has been held|252|
|current_hold_time|integer|the length of time the current user has held the nft|253|
|date_of_birth|string|timestamp of the date the nft was cast|1632873600000|
|past_owners|string|number of users who have handled the nft (including current users). (including current users)|2|
|max_price|float|the highest price of nft(USD)|14230.777|
|min_price|float|the lowest price of nft(USD)|14230.777|
|avg_price|float|the average price of nft(USD)|14230.777|
|number_of_sales|integer|number of times this nft was sold|1|
|latest_price|float|current latest price(USD)|14230.777|
|owner_transfer_time|string|time of transfer|1632873600000|
|owner_address|string|address of the user currently holding the nft|0x4f94fa697f4eaa8c25a097fa0c9d254cdb114465|
|latest_amount|integer|current latest price|5|
|avg_amount|integer|the avg amount of this NFT Collection today|5|
|min_amount|integer|the min amount of this NFT Collection today|5|
|max_amount|integer|the max amount of this NFT Collection today|5|


**Nft_transactions Model**

| Field Name |Field Type| Description | Example |
|:------------:|:-------------:|:-------------:|:---------:|
|chain|string|the chain of this NFT Collection|Ethereum|
|block_timestamp|string|timestamp of the block where this transfer was in|1654901555000|
|transaction_hash|string|hash of the transaction|0x09893622371640164d352272aec4876c40be5bfcbc98c334067c351b4a68ccaa|
|log_index|integer|log index in the transaction receipt|178|
|collection_name|string|name of nft collection|Foundation (FND)|
|protocol_slug|string|abbreviation of the protocol|fnd|
|contract_address|string|address of contract|0x3b3ee1931dc30c1957379fac9aba94d1c48a5405|
|nft_token_id|float|id of the nft token|120213|
|marketplace|string|marketplace of the transaction|OpenSea|
|from_address|string|address of the sender|0x005052a468069b40a239b9f0be7f6b98cdacb096|
|to_address|string|address of the receiver|0xe052113bd7d7700d623414a0a4585bcae754e9d5|
|amount|float|amount of tokens transferred / id of the token transferred|0.03|
|value_currency|string|value of currency|0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee|
|value|float|value|49.811218|
|marketplace_contract_address|string|address of marketplace contract|0x7f268357a8c2552623316e2562d90e642bb538e5|
|business_type|string|type of business|sales|

## NFT

### Get the detail daily stats of each NFT Collection
Method: post  
Path: /api/nft/nft_collection_daily_stats  
Header: 'FP-API-KEY: YOUR_ACCESSKEY'    
Parameters: 
* chain(string): The chain of this NFT Collection, eg: 'Ethereum'
* contract_address(string): The contract address of this NFT Collection, eg:'0x00000633df1228868270badb2b812e12e13fdb91'
* on_date(string): The date of this record, Default yesterday, eg: '2022-01-01'
* limit(integer): Page size, Defaults to 1000, capped at 2000, eg: 100
* offset(integer): The offset for pagination eg:120

Request Body
```json
{
    "chain": "Ethereum",
    "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
    "on_date": "2022-06-10",
    "limit": 1,
    "offset": 0
}
```

Result 
```json
{
    "message": "success",
    "code": 0,
    "data": [
        {
            "protocol_slug": "fnd",
            "chain": "Ethereum",
            "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
            "on_date": "1654819200000",
            "collection_name": "Foundation (FND)",
            "number_of_mint": 0,
            "number_of_transactions": 45,
            "number_of_burn": 0,
            "number_of_sale_transactions": 3,
            "number_of_transfer_transactions": 36,
            "number_of_sellers": 3,
            "number_of_buyers": 1,
            "number_of_holders": 17858,
            "volume": 132.82993,
            "market_cap": 3844896.8,
            "total_supply": 132928,
            "liquidity": 0.000022999999999999997,
            "avg_amount": 0.026667,
            "avg_price": 44.276642,
            "max_amount": 0.03,
            "min_amount": 0.02,
            "max_price": 49.811218,
            "min_price": 33.207481
        }
    ]
}
```

### Get information of nft collection
Method: post  
Path: /api/nft/nft_collection_info  
Header: 'FP-API-KEY: YOUR_ACCESSKEY'    
Parameters: 
* chain(string): The chain of this NFT Collection, eg: 'Ethereum'
* contract_address(string): The contract address of this NFT Collection, eg:'0x00000633df1228868270badb2b812e12e13fdb91'
* limit(integer): Page size, Defaults to 1000, capped at 2000, eg: 100
* offset(integer): The offset for pagination eg:120

Request Body
```json
{
    "chain": "Ethereum",
    "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
    "limit": 1,
    "offset": 0
}
```                
Result 
```json
{
    "message": "success",
    "code": 0,
    "data": [
      {
        "chain": "Ethereum",
        "protocol_slug": "fnd",
        "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
        "collection_name": "Foundation (FND)",
        "logo": "https://lh3.googleusercontent.com/uUdrzISpIJJVRbm_g6mmu-TUaOERBbPJcNA8KeuwI1HNgXy8Kje3c2XhoMIndnPmyono9NUJE8A2_bTd95iqAcjo9pyy-e47flJy=s120"
      }
    ]
}
```

### Get the metrics for different nft
Method: post  
Path: /api/nft/nft_latest_stats  
Header: 'FP-API-KEY: YOUR_ACCESSKEY'    
Parameters: 
* chain(string): The chain of this NFT Collection, eg: 'Ethereum'
* contract_address(string): The contract address of this NFT Collection, eg:'0x00000633df1228868270badb2b812e12e13fdb91'
* limit(integer): Page size, Defaults to 1000, capped at 2000, eg: 100
* offset(integer): The offset for pagination eg:120  

Request Body
```json
{
    "chain": "Ethereum",
    "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
    "limit": 1,
    "offset": 0
}
```                
Result 
```json
{
    "message": "success",
    "code": 0,
    "data": [
      {
        "chain": "Ethereum",
        "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
        "protocol_slug": "fnd",
        "nft_token_id": 66948,
        "longest_hold_time": 204,
        "current_hold_time": 50,
        "date_of_birth": "1627776000000",
        "past_owners": 4,
        "max_price": 273.46579,
        "min_price": 261.37366,
        "avg_price": 267.41974,
        "number_of_sales": 2,
        "latest_price": 273.46579,
        "owner_transfer_time": "1650412800000",
        "owner_address": "0x188b79d5ab7a27bb098d740e51c5253cf375be86",
        "latest_amount": 0.089,
        "avg_amount": 0.094,
        "min_amount": 0.089,
        "max_amount": 0.099
      }
    ]
}
```

### Get the transactions of different nft series
Method: post  
Path: /api/nft/nft_transactions  
Header: 'FP-API-KEY: YOUR_ACCESSKEY'    
Parameters: 
* chain(string): The chain of this NFT Collection, eg: 'Ethereum'
* contract_address(string): The contract address of this NFT Collection, eg:'0x00000633df1228868270badb2b812e12e13fdb91'
* block_timestamp(string): The date of this record, Default yesterday, eg: '2022-01-01'
* limit(integer): Page size, Defaults to 1000, capped at 2000, eg: 100
* offset(integer): The offset for pagination eg:120  

Request Body
```json
{
    "chain": "Ethereum",
    "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
    "block_timestamp": "2022-06-10",
    "limit": 2,
    "offset": 1
}
```                
Result 
```json
{
    "message": "success",
    "code": 0,
    "data": [
      {
        "chain": "Ethereum",
        "block_timestamp": "1654901555000",
        "transaction_hash": "0x09893622371640164d352272aec4876c40be5bfcbc98c334067c351b4a68ccaa",
        "log_index": 178,
        "collection_name": "Foundation (FND)",
        "protocol_slug": "fnd",
        "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
        "nft_token_id": 120213,
        "marketplace": "OpenSea",
        "from_address": "0x005052a468069b40a239b9f0be7f6b98cdacb096",
        "to_address": "0xe052113bd7d7700d623414a0a4585bcae754e9d5",
        "amount": 0.03,
        "value_currency": "0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
        "value": 49.811218,
        "marketplace_contract_address": "0x7f268357a8c2552623316e2562d90e642bb538e5",
        "business_type": "sales"
      },
      {
        "chain": "Ethereum",
        "block_timestamp": "1654901813000",
        "transaction_hash": "0x123256bdff0cf6aed1ed5a4024b4969e672a9606511a51c420aebda2c62f27dc",
        "log_index": 69,
        "collection_name": "Foundation (FND)",
        "protocol_slug": "fnd",
        "contract_address": "0x3b3ee1931dc30c1957379fac9aba94d1c48a5405",
        "nft_token_id": 19953,
        "marketplace": "OpenSea",
        "from_address": "0x5e1ad5ff09291aa6512e6d4fddbbb604549dc54c",
        "to_address": "0xe052113bd7d7700d623414a0a4585bcae754e9d5",
        "amount": 0.03,
        "value_currency": "0xeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee",
        "value": 49.811218,
        "marketplace_contract_address": "0x7f268357a8c2552623316e2562d90e642bb538e5",
        "business_type": "sales"
      }
    ]
}
```