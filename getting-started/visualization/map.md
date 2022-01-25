# Map

When you select the Map visualization setting, Metabase will automatically try and pick the best kind of map to use based on the table or result set. Here are the maps that Metabase uses:

Coming soon.

**United States Map**. Creating a map of the United States from your data requires your results to contain a column that contains names of states or two-letter state codes. This lets you do things like visualize the count of your users broken out by state, with darker states representing more users.&#x20;



World Map. To visualize your results in the format of a map of the world broken out by country, your result must contain a column with two-letter country codes. (E.g., count of users by country.)

![](<../../.gitbook/assets/image (18).png>)

**Pin Map**. If your results contain a latitude and longitude field, Metabase will try to display the results as a pin map of the world. Metabase will put one pin on the map for each row in your table, based on the latitude and longitude fields. You can try this with the Sample Dataset that’s included in Metabase: start a new question and select the People table, use raw data for your view, and choose the Map option for your visualization. You’ll see a map of the world, with each dot representing the latitude and longitude coordinates of a single person from the People table.

![](<../../.gitbook/assets/image (19).png>)

When you open up the Map options, you can manually switch between a region map (e.g., United States) and a pin map. If you’re using a region map, you can also choose which field to use as the measurement, and which field to use as the region (e.g., State or Country).

It also allows administrators to add custom region maps via GeoJSON files through the Metabase Admin Panel.
