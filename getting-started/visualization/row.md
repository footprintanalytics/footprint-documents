# Row chart

If you’re trying to group a number by a column that has a lot of possible values, like a Vendor or Product Title field, try visualizing it as a row chart. Footprint will show you the bars in descending order of size, with a final bar at the bottom for items that didn’t fit.

![](<../../.gitbook/assets/image (12).png>)

**Histograms**

If you have a bar chart like Number of Users by Age, where the x-axis is a number, you’ll get a special kind of chart called a histogram, where each bar represents a range of values (called a “bin”). Note that Footprint will automatically bin your results any time you use a number as a grouping, even if you aren’t viewing a bar chart. Questions that use latitude and longitude will also get binned automatically. By default, Footprint will automatically choose a good way to bin your results. But you can change how many bins your result has, or turn the binning off entirely, by clicking on the area to the right of the column you’re grouping by:



![](<../../.gitbook/assets/image (14).png>)
