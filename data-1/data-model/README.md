# 📑 Data model

## Design concept of **table**

### **Reduce join tables**

With the most frequently used combination of **protocol\_slug+chain**, you can quickly find the data you want in multiple tables.

### **Reduce the cost of understanding**

1. Consistent presentation of multiple fields in different tables, reduces the cost of understanding, e.g. contract address, which is called by one name in all tables.
2. For example, with the suffix **daily\_stats**, you know it is a statistical table updated by day.
3. For example ,with the suffix **info** ,you know it is a static information data table.

### **Solve the problem of importing data that cannot be associated**

Provide basic information tables with **\_info** suffix to association of internal and external table.

## Data naming conventions

### **Table & field naming convention**

1. Table name and fields name must be in Lowercase.
2. Underscores separate the distinct terms that define the Table or Column as per the standard conventions.
3. All table names must be in plural form. table names must have only A to Z, 0 to 9, and underscore (\_) characters.
4. Table names can have multiple underscores.

### **Table naming convention**

1. Prefix
   * **ud\_** : means user define, data contributed by the community.
2. Suffix
   * **\_info** : represents the base information table maintained by Footprint and can be used as a hub for data association.
   * **\_daily\_stats** : the data in the table are aggregated by day.
   * **\_token\_transfers** : flow records of data chain tokens.
   * **\_transactions** : represents transaction that occurs on the blockchain, and the hash value represents its uniqueness.
3. Special Mark
   * **Beta:** data accuracy, stability, data period, update frequency,etc of this table is still on working.

### **Field naming convention**

1. Chain
   * **chain** : The fields chained within the system are uniformly called chain.
2. Protocol
   * **protocol\_slug** : The naming of protocols within the system, the usual user appearance associations and queries.
3. Token
   * **token\_slug** : The token is uniquely identified within the Footprint.
4. Wallet
   * **address** : Internally, the part of the system that uniquely identifies the user is called address, not user or account, etc. There are two types of address:
     * wallet\_address
     * contract\_address
5. NFT
   * **nft\_token\_id** : Unique identifier in the same NFT collection.
6. Transaction
   * **value** : Represents the flow of value in a transaction, usually in US dollars, as shown in value\_currency.
   * **number\_of** : Number of integers, such as number of addresses, number of transactions, etc.
   * **amount** : Represents mathematical units that contain decimal types, such as token amount , volume , tvl , etc.
   * **value\_currency** : Unit of value calculation, if the field is not present in the table, it means that the value is calculated in usd.
