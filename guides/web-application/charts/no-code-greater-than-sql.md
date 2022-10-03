# No code -> SQL

Footprint is built on a visualisation and plotting engine called Metabase:

{% embed url="https://www.metabase.com/" %}
Metabase official website
{% endembed %}

Architecturally, Metabase is implemented in such a way that whatever chart is created in an easy-to-use UI, under the hood, it is first converted to SQL and subsequently sent to the server.&#x20;

{% hint style="info" %}
It is possible to convert any chart created in UI to SQL form, but in the opposite direction it is possible only in case of simple queries&#x20;
{% endhint %}

Next, there will be a demonstration of the process of converting a graph previously created using the drag-and-drop method into an SQL form.

<figure><img src="../../../.gitbook/assets/output (1).gif" alt=""><figcaption><p>Video explanation</p></figcaption></figure>

Following is the step-by-step explanation of the whole workflow:

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.44.37.png" alt=""><figcaption><p>From Home page press <code>Create</code> button</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.45.28.png" alt=""><figcaption><p>In the modal widow select <code>New chart</code></p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.47.37.png" alt=""><figcaption><p>Create a query with a simple drag-and-drop interface (the example above is demonstrating the number of nft transactions performed within last 7 days and grouped by the collection slug)</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.48.30.png" alt=""><figcaption><p>Press three dots in the top right corner -> press <code>View the SQL</code> button</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.49.12.png" alt=""><figcaption><p>The SQL code will be displayed in the modal window</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screenshot 2022-09-30 at 14.49.52.png" alt=""><figcaption><p>Additionally a query could be converted to the SQL form</p></figcaption></figure>
