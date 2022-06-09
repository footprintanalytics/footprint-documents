# Upload Data to Footprint By Using the API

Footprint supports cross analysis of on-chain and off-chain data. Complete the steps described in the rest of this page to upload your off chain data by using API.

****

### **Step1: Generate developer auth key**

1. **Generate an auth key**\
   On the top right hand-side of the website, click on **your avatar.** A pop-up menu will appear. And then click on **Account Settings.**

![](<../.gitbook/assets/0 (6)>)

2\. In the Developer's settings, click on the **Generate Anth Key** button to get an **auth key.**

![](<../.gitbook/assets/1 (3)>)

3\. Use the auth key\
Add the authentication: auth key to the header, for example:

```
{
  	"headers": {
 "authentication": "Your Auth Key"
 }
}
```

### **Step2: General Instructions for Calling the API**

1. **Interface url**\
   https://www.footprint.network/api/v1/custom/data/upload

****

### **Step3: Data Interaction Specification**

1. Use HTTPS protocol for data communication;&#x20;
2. Use POST method to send requests;
3. The data return format uses JSON format.

### **Step4: Upload your data**

1. **Add custom data**
   * Interface name
     * POST /api/v1/custom/data/upload
2. **Request parameter data description**
   * Request parameter

| **Field name**   | **Type** | **Required** | **Description**                                                                                          |
| ---------------- | -------- | ------------ | -------------------------------------------------------------------------------------------------------- |
| tableName        | String   | Yes          |                                                                                                          |
| tableFieldSchema | Array    | Yes          | Header definition                                                                                        |
| tableDate        | Date     | No           |                                                                                                          |
| updateForce      | Boolean  | No           | The default is false, if uploading data will overwrite existing data, this value needs to be set to true |
| tableData        | Array    | Yes          | Table data                                                                                               |

* tableFieldSchema

| **Field name** | **Type** | **Required** | **Description** |
| -------------- | -------- | ------------ | --------------- |
| name           | String   | Yes          | Field name      |
| type           | Enum     | Yes          |                 |

3\. **Example**

```
{
  "tableName": "your_table_name",
  "tableFieldSchema": [{
    "name": "chain",
    "type": "STRING"
  }, {
    "name": "time",
    "type": "DATETIME"
  }],
  "updateForce": false,
  "tableData": [{
    "chain": "BSC",
    "time": "2022-01-01 12:00:00"
  }, {
    "chain": "Polygon",
    "time": "2022-01-01 12:00:00"
  }]
}
```



4\. **Response data description**

| Field name | Type   | Required | Description               |
| ---------- | ------ | -------- | ------------------------- |
| code       | String | Yes      | tatus code code=0,success |
| message    | String |  No      | description               |

* **Example**

```
{
  "code": 0,
  "message": "success"
}
```



### **Step 5. Data Display**

The final uploaded data will be under the Personal Upload directory on the left column of the create chart page.\
<img src="../.gitbook/assets/2 (4)" alt="" data-size="original">
