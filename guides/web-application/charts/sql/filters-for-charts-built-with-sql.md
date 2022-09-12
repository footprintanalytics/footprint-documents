# Filters for charts built with SQL

### Dashboard filter case steps

* First, type \{{variable\_name\}} in the SQL statement. For example "`select * from defi_protocol_daily_stats [[where {{chain}}]]`".

<figure><img src="../../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

* Second, set the parameters in the right sidebar.
* Third, you must select the variable type as `field filter` and select the associated field.&#x20;

<figure><img src="../../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

* Finally, you can associate the filter field of the chart in the dashboard.

### Another use case steps

* First, type \{{variable\_name\}} in the SQL statement. For example "`select * from defi_protocol_daily_stats [[where chain={{chain}}]]`".

<figure><img src="../../../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

* Second, set the parameters in the right sidebar.
* Third, you must select the variable type as `Text` .&#x20;
* Finally, you can type `Ethereum` in the filter input box and run it, and you can see that the result set has been filtered with `Ethereum`.

<figure><img src="../../../../.gitbook/assets/image (4) (3).png" alt=""><figcaption></figcaption></figure>
