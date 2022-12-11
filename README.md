# BA6 Final Project: Number of Internet Users in North America Over Time

Project Description:
An interactive web application which shows a choropleth map of countries in North America, including Canada, USA, Mexico, and Greenland. The application features a time slider which allows the user to change the year between the ranges of 2000 and 2020, which updates the choropleth map to display the corresponding number of internet users in each country for the given year.
<br>
<br>
Project Goal: The goal of this application was to illustrate how relatively recently the internet has integrated into society to become a standard of everyday life. Using the time slider, the user is able to see how the number of internet users in North America has grown exponentially across just two decades. The user is also able to see that the US has been one of the quickest countries to adopt the internet, and that this standard of internet access is not universal, and there are disparities of internet access between countries, even just within this continent. For example, when the user opens the web application, it is easy to notice that the US already has significantly more users than the other countries in North America, even in the early year of 2000. As the time slider increases the year for the map, the US is also seen to have a very high rate of increase, and still has the most internet users in North America today. This information therefore helps people living in industrialized countries to realize that society depends so heavily on internet access nowadays, however, the internet is still a relatively new invention, and many countries around the world are still lacking this tool that many of us take for granted.
<br>
<br>
Project Process:
We have met several difficulties when building the map of this project. The first was processing data. There are several datasets from the data source, we select the most suitable ones for our project and download them. However, these datasets are too large for our project. Thus we first fiter the part that we really need. After cleaning thousands lines of data, we got what we have in our repo now. All of these datasets were in csv format, but obviously, geojson is the format appropriate for this project. That is to say, we have to try converting the csv datasets we have to geojson datasets. We have tried many ways doing that and finally, considering the goal and content of this project, we chose to add the csv data to continent shapefile manually. That took us certain of time as the amount of csv data is twenty years in four countries. The second difficulty we met was filtering the map based on the year changing with user moving the slider. Even though we got mapbox template to reference, we are doing different types of map to the template, which means we need to think oursevles to code the changing filter. The third difficulty we met was how to define the appropriate legend. Because Greenland's data in some way exist as an outlier comparing to other countries, in order to balance the color of Greenland and the color of other three countries, we did make some efforts. The last difficulty was the custom style of base map, it's not hard making the custom map, but it was hard to use it publically. We didn't know that the mapbox need to be updated to latest version to use the custom map, which took us a while to figure out.
<br>
<br>
Web Application link: https://raeoyw.github.io/BA6FinalProject/index.html

Screenshots:
<img width="1422" alt="image" src="https://user-images.githubusercontent.com/115133002/206929481-3d971b58-c4a0-47f5-85e2-455717d48343.png">

<img width="1427" alt="image" src="https://user-images.githubusercontent.com/115133002/206929506-7835febf-7894-4abc-bfcc-8a81e715e8ee.png">
<br>
<br>
Main functions:
The user is able to zoom and pan around the map, due to the use of map box, and adjust the time slider to view the number of internet users in each country for the years between 2000 and 2020.
<br>
<br>
data sources:
Data for the number of internet users by country over time: https://ourworldindata.org/internet
Data for Geojson geometry file: https://geojson-maps.ash.ms/
<br>
<br>
Applied Libraries:
<br>
- Mapbox: A map server which offers a wide selection of interactive base maps that can be loaded into web applications using an access token for geographic visualizations.
<br>
<br>
Applied Web Services
<br>
- Github: Used for hosting our web application and uploading our files for collaboration
<br>
- Basemap: Used alongside Mapbox to create the basemaps seen in our web application
<br>
- Geo Data Merger: Used for combining Geojson files with CSV data files to assign properties to objects (https://funkeinteraktiv.github.io/geo-data-merger/).
<br>
<br>

Acklowledgements:
We would like to acklowledge that this web application was created as a project for the University of Washington GEOG 495: Web GIS class instructed by professor Bo Zhao. The authors of this web application are Rae Ouyang, Omar Romero, and Ethan Liu.

