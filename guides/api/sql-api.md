# SQL API

Any request that can be executed through our web UI (see [web-application](../web-application/ "mention")) can be called programmatically. This instruction is devoted to the description of authorization, the formation of the query and sending of appropriate requests for the purpose of integration on the side of client applications.

{% hint style="info" %}
The simplest way to come up with valid SQL query is to have a chart created via the drag-and-drop interface and consequently convert it to SQL within Footprint web application. The step-by-step example how to achieve it could be found in [no-code-greater-than-sql.md](../web-application/charts/no-code-greater-than-sql.md "mention")
{% endhint %}

## Quickstart

The following Hoppscotch (an open-source, easy-to-use API development ecosystem) collection could be used to quickly start executing the query using Footprint SQL API:

{% file src="../../.gitbook/assets/Footprint SQL API.json" %}
Hoppscotch collection file
{% endfile %}

<figure><img src="../../.gitbook/assets/output.gif" alt=""><figcaption><p><strong>Video guide</strong></p></figcaption></figure>

**Step 1**. Download the file above to your local machine

**Step 2**. Proceed to Hoppscotch official client application:

{% embed url="https://hoppscotch.io/" %}
Hoppscotch official client application
{% endembed %}

**Step 3**. Import the previously downloaded file:

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-03 at 10.54.49.png" alt=""><figcaption><p>Import collection workflow</p></figcaption></figure>

**Step 4**. Complete the authorisation process:

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-03 at 10.57.03.png" alt=""><figcaption><p>Authorisation process completed</p></figcaption></figure>

**Step 5**. Execute the query:

<div>

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-03 at 10.59.47.png" alt=""><figcaption><p>Query body</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2022-10-03 at 10.59.55.png" alt=""><figcaption><p>Query header</p></figcaption></figure>

</div>

## Step-by-step guide

{% swagger method="post" path="/session" baseUrl="https://www.footprint.network/api" summary="Authorisation" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="username" type="String" required="true" %}
footprint.network username
{% endswagger-parameter %}

{% swagger-parameter in="body" name="password" type="String" required="true" %}
footprint.network password
{% endswagger-parameter %}

{% swagger-parameter in="body" name="remember" type="Boolean" required="false" %}
Remember session?
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
```javascript
{
    "id": "metebase.SESSION"
}
```
{% endswagger-response %}

{% swagger-response status="401: Unauthorized" description="" %}
```javascript
{
   "errors":{
      "password":"The password is invalid"
   }
}
```
{% endswagger-response %}
{% endswagger %}

Once the authorisation is successful (HTTP response :green\_circle: `200: OK` with Metabase session id is received), it is possible to execute any query via any HTTP client.

{% swagger method="post" path="/dataset" baseUrl="https://www.footprint.network/api/v1/database" summary="SQL query execution" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="cookie" type="String" required="true" %}
metabase.SESSION=bf400df1-2616-4b89-afd5-a05ace1xxxxxx
{% endswagger-parameter %}

{% swagger-parameter in="body" name="type" type="Integer" required="true" %}
Always 

`native`
{% endswagger-parameter %}

{% swagger-parameter in="body" name="native" type="String" required="true" %}
Object containing 

`query`

 sub-object
{% endswagger-parameter %}

{% swagger-parameter in="body" name="native.query" type="String" required="true" %}
SQL query to be executed
{% endswagger-parameter %}

{% swagger-parameter in="body" name="database" type="Integer" required="true" %}
Always 

`3`
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
code: -1 => auth fail

```javascript
{
    "message":"auth fail",
    "code": -1
}
```

code: 503 => unknown error

```javascript
{
    "code":503,
    "message":"The first argument must be of type string or an instance of Buffer, ArrayBuffer, or Array or an Array-like Object. Received undefined"
}
```
{% endswagger-response %}

{% swagger-response status="201" description="" %}
```javascript
{
    "data": { ... }
}
```
{% endswagger-response %}
{% endswagger %}

A complete example of query execution using `curl` is presented in the following example:

```bash
curl -X POST \
  https://www.footprint.network/api/v1/database/dataset \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'cookie: metabase.SESSION= {{ authenticate using `api/session` endpoint to get the metabase id }}' \
  -d '{
	"type":"native",
	"native":{
		"query":"select * from `protocol_daily_stats` limit 10"
	},
	"database":3
}'
```
