# Norman Sicily Project. 
Folders contain separate GeoJSON files
Norman Sicily Project
	Monasteries can give an indication on the historical time period in which the monastery was created or attested. Religion played a huge part in Sicilian culture during the Norman Conquest. This can be seen throughout the monasteries across Sicily, given their dedications at the time of attestation. The monasteries of the Norman Kingdom of Sicily contain much of Sicilian History. Depending on the monastery, we can be looking at a historical monument from 1000-1300 AD. This can affect the history within a given monastery because different monasteries were subject to different rulers. One of the most prominent rulers is King Roger II. He was accredited for creating a successful government with the Norman Conquest. He ruled between the years of 1130-1154 AD. There will be close examination of how the data is affected by the rule of King Roger II. 

The data set:
	The data set provided includes different fields, such as dedication, reign, and order. The time period being worked with is from 1000-1300 AD. Differences between the distributions of monasteries will be recorded in visualizations (map images). Within a 300 year time frame, there can be differences influenced by the era and the ruler. This will be further explored with the given data sets. Manipulating the data sets allow for the visualization of clustering occurring in different parts of Sicily. 
Certain data sets which were visualized:
•	Order
•	Reign
•	Dedication
•	Time Period
•	Seismic Class
Monasteries were classified with these field in order to visualize the distribution. Maps were also created to visualize where the distribution is taking place. 

Historical Significance:
	Depending on the time period, monasteries can have significant differences under certain rule. Part of the GIS analysis of this project will also look at separating the dataset in to three categories; before Roger II, Roger II, after Roger II. The reason why we separate the data depending on Roger II is because he was a prominent ruler for Norman Sicily. 
GIS analysis:
	The dataset is used in QGIS in order to create visualizations which can highlight different attributes in the dataset. First, the basemap is downloaded for commune and province from the Italian government website. These are the basemaps we will work with in order to visualize the data. Now the separation of the datasets is created by extracting what we visually want to see on the map. For example, if we want to separate the monasteries based on seismic class, we can visualize which monasteries are in seismic zone 3. We do this separation, not only for the seismic attribute, but for other attributes as well. 
(ADD IMAGES OF MAPS HERE)
 
	When selecting by attributes, we are also able to isolate other columns in the dataset to highlight other significant differences in monasteries. One attribute we used for separation was the dedications. Given the historical context of Norman Sicily, dedications is an important field to isolate. 
(Add dedication map)
	This map shows the separation of dedication with the monasteries. We also performed this function with other columns in the dataset. All of the datasets are downloaded as geojson files and uploaded on to github. When clicking on each point, the file will then show you a list of information given the point you click on. 

Statistical analysis:
	The data set was used to calculate different statistics depending on the field. For example, simple statistics can be calculated to evaluate how many Null (or missing) values are found within a given field. 
	The installation of different libraries allows for the creation of different types of maps using R studio. In order to create said maps, a get_map function has to be used in which we specify which region we want to work with. For the purpose of this project, the region selected is Sicily. This allows us to have a base map to work with. The beginning stages for code call for us to install different packages in order to use different functions on the dataset.
	We begin to write in clustering functions to cluster different monasteries based on seismic classification to see if there is any clustering which occurs. 
(INSERT CLUSTERING FIGURE HERE)
What we can also do with this data is separate it depending on different attributes. For example, we can create heat maps which can show which areas have higher seismic classification values or we can also calculate which areas had more dedications than other areas. With the code, we are able to create chloropleth maps on the province level. Using GIS, we are able to separate the data in commune level. The problem with separating the maps using commune level is that it does become messy since there is more separation which occurs. It is more accurate to separate different attributes depending on the commune level but it is not as visually appealing as separating it by the province level.  
(INSERT CHLOROPLETH MAP HERE) 
The other interesting thing we are able to do with the code is create an R shiny app which becomes interactive for the use of the different types of visualization you can do with the dataset. It becomes convenient because the tab function allows us to visualize the datasets in different tabs. 
