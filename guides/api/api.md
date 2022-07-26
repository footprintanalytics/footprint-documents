# ⚙ Upload API

## **Generate developer auth key**

1. **Generate an auth key**\
   On the top right hand-side of the website, click on **your profile.** A pop-up menu will appear. And then click on **Account Settings.**

![](<../../.gitbook/assets/0 (6)>)

2\. In the developer's settings, click on the **Generate Anth Key** button to get an **auth key.**

![](<../../.gitbook/assets/1 (5)>)

3\. Use the auth key\
Add the authentication: auth key to the header, for example:

```json
{
   "headers":{
      "authentication":"Your Auth Key"
   }
}
```

## **Methods**

### **Upload data**

{% swagger method="post" path="" baseUrl="https://www.footprint.network/api/v1/custom/data/upload" summary="Upload data to Footprint" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" required="true" name="API-KEY" type="String" %}
Authorisation key obtained from profile
{% endswagger-parameter %}

{% swagger-parameter in="body" name="tableName" type="String" required="true" %}
The name of table
{% endswagger-parameter %}

{% swagger-parameter in="body" name="tableFieldSchema" required="true" type="Array" %}
Header row of uploaded table (see schema below)
{% endswagger-parameter %}

{% swagger-parameter in="body" name="tableDate" type="Date" required="false" %}
Date of table creation
{% endswagger-parameter %}

{% swagger-parameter in="body" name="updateForce" type="Boolean" required="false" %}
The default is false, if uploading data will overwrite existing data, this value needs to be set to true
{% endswagger-parameter %}

{% swagger-parameter in="body" name="tableData" type="Array" required="true" %}
Table data itself
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
  "code": 200,
  "message": "success"
}
```
{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="" %}
```javascript
{
  "code": 200,
  "message": "internal_server_error"
}
```
{% endswagger-response %}
{% endswagger %}

`tableFieldSchema`

| **Field name** | **Type** | **Required** | **Description** |
| -------------- | -------- | ------------ | --------------- |
| name           | String   | Yes          | Field name      |
| type           | Enum     | Yes          | Field type      |

#### Example

```json
{
   "tableName":"your_table_name",
   "tableFieldSchema":[
      {
         "name":"chain",
         "type":"STRING"
      },
      {
         "name":"time",
         "type":"DATETIME"
      }
   ],
   "updateForce":false,
   "tableData":[
      {
         "chain":"BSC",
         "time":"2022-01-01 12:00:00"
      },
      {
         "chain":"Polygon",
         "time":"2022-01-01 12:00:00"
      }
   ]
}
```
