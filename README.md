# NYC_Urban_Livability
A multi-factor analysis on rent, noise &amp; crime across New York City using Machine Learning techniques including Time Series Analysis, Cluster Analysis and Spatial Analysis.

# 1) How are rent prices expected to change in the next two years across New York City?
This study utilizes StreetEasy’s dataset containing monthly data on the median asking rent in New York City. 

## Methodology
To obtain predictions with the highest accuracy, we compare the performance of simple forecasting, exponential smoothing, ETS and ARIMA models on the testing data. The Holt Winter multiplicative method closely mimics the testing data and provides the lowest RMSE score at 96.63.

2) How do the noise complaint types vary across neighborhoods in New York City?
3) How do the crimes vary across neighborhoods in New York City?

## Findings
The forecast shows that the median rental price in January 2023 starts at $3,410, and by December 2025, it rises to $3,682.

# 1) How do the noise complaint types vary across neighborhoods in New York City?
This study utilizes NYC Open Data’s dataset containing roughly 6.5 million complaints. 

## Methodology
Cluster analysis is used to group neighborhoods on the basis of the various types of noise complaints. This helps identify the characteristics of a given neighborhood and determine whether it is suitable for a residents requirements. A K-means model is selected for this analysis, as it is scalable and easy to implement. 

## Findings
Three kinds of neighborhoods were identified. Cluster 1 has the highest levels of noise complaints, indicating high population density and commercial zones with significant street activity. Cluster 2 has neighborhoods with a small mix of residential and commercial areas. Cluster 3 has  relatively moderate levels from streets and sidewalks indicating that they are not very densely populated. However commercial, helicopter and random noises are significantly higher here than in the other two clusters.

# 1) How do the crimes vary across neighborhoods in New York City?
Using the NYC open data and the Google Maps API, we evaluate the crime levels and types across the city.

## Methodology
get_map() to fetch maps from Google Maps to serve as a base layer for the spatial visualization. It sets the location, zoom level, and scale for the map of New York City. ggmap() then initializes the plotting of the map object obtained from get_map(). Finally, we used functions such as theme(), and guides() to modify the appearance of the plot.

## Findings
Crime is more concentrated in Manhattan, Southern Bronx & Central Brooklyn. Felonies were the most common category of crime
Displaying the frequency of crimes as color-coded points allows for immediate visual identification of areas with higher crime densities. For spatial analysis, this map can help identify hotspots for specific types of crime and observe any geographic patterns or clusters. For example, a high concentration of red points in a particular area would indicate a region with a high incidence of felonies.




