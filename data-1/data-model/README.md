# 📑 Data Model

## Design Concept of Data Model

### **1. Reduce join tables**

With the most frequently used combination of **protocol\_slug+chain**, you can quickly find the data you want in multiple tables.

### **2. Reduce the cost of understanding**

1. Consistent presentation of multiple fields in different table, reduces the cost of understanding, e.g. contract address, which is called by one name in all tables.
2. For example, with the suffix **daily\_stats**, you know it is a statistical table updated by day.
3. For example ,with the suffix **info** ,you know it is a static information data table

### **3. Solve the problem of importing data that cannot be associated.**

Provide basic information tables with **\_info** suffix to association of internal and external table

## Data Regulations

### **1. Table naming regulations**

1. Prefix
   1. **ud\_** : means user define, data contributed by the community.
2. Suffix
   1. **\_info** : represents the base information table maintained by Footprint and can be used as a hub for data association.
   2. **\_daily\_stats** : the data in the table are aggregated by day.
   3. **\_token\_transfers** : flow records of data chain tokens.
   4. **\_transactions** : represents transaction that occurs on the blockchain, and the hash value represents its uniqueness.

### **2. Field naming regulations**

1. Chain
   1. **chain** : The fields chained within the system are uniformly called chain.
2. Protocol
   1. **protocol\_slug** : The naming of protocols within the system, the usual user appearance associations and queries.
3. Token
   1. **token\_slug** : The token is uniquely identified within the Footprint
4. Wallet
   1. **address** : Internally, the part of the system that uniquely identifies the user is called address, not user or account, etc. There are two types of address:&#x20;
      1. wallet\_address&#x20;
      2. contract\_address
5. NFT
   1. **nft\_token\_id** : Unique identifier in the same NFT collection
6. Transaction
   1. **value** : Represents the flow of value in a transaction, usually in US dollars, as shown in value\_currency&#x20;
   2. **number\_of** : Number of integers, such as number of addresses, number of transactions, etc.&#x20;
   3. **amount** : Represents mathematical units that contain decimal types, such as token amount , volume , tvl , etc.&#x20;
   4. **value\_currency** : Unit of value calculation, if the field is not present in the table, it means that the value is calculated in usd

