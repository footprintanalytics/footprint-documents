# Data structure

![Footprint data layers](<../../.gitbook/assets/Footprint data layer.jpg>)

Footprint has 3 layer data:

### **Bronze**

Raw untransformed unmodified data. Providing detailed records of all activities on the blockchain.

### **Silver**

The raw Bronze data is transformed into sets of data that adds additional values. This can imply replacements of codes to meaningful values, adding sanity constraints, filtering-out unneeded information, etc.

Such as `ethereum_tranactions`, `ethereum_token_transfer`, `protocol_transactions`, `contract_info` and etc.

### **Gold**

Well-constructed dataset ready for analysis. Presented in such a way including aggregations, joins and merges, encoding, etc.

Such as `dex_pool_liquidity_daily_stats`,`lending_pool_daily_stats`,etc.

***
