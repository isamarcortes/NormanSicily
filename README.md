# Norman Sicily Project. 
Folders contain separate GeoJSON files
The Norman Sicily Project's Monastic Data Set
	
	The data set provided, drawn almost exclusively from Lynn White's landmark study, _Latin Monasticism in Norman Sicily_ (1938), includes a large number of fields. The time period the data span is ca. 1060-1194 AD. Differences noted in the distributions of monasteries were recorded in visualizations (map images). Within the 134-year chronological span, there were differences influenced by space, time and people. These were explored in the data sets; manipulating them allowed for the visualization of clustering that occurred in different parts of the island.
	
Specific data subsets which were visualized include:
•	Order
•	Reign
•	Dedication
•	Time Period
•	Seismic Class
Monasteries were classified by these fields in order to visualize distributions. Maps were also created to visualize where the distributions were located. 

Historical Significance:
	Depending on the time period, monastic foundations can be significantly shaped by particular rulers. Part of the GIS analysis of this project looked at separating the dataset into three categories: before Roger II's reign (pre-1112), during Roger II's reign (1112-1154) and after Roger II's reign (1154-1194). The reason why Roger II's reign was chosen as a delimiter is because it was both consequential and long, making up almost a full third of Sicily's Norman period.

GIS Analysis:
	The dataset was used in QGIS in order to create visualizations which can highlight different attributes. First, a basemap was downloaded for municipalities (comuni) and provinces from the Italian government's website. These are the basemaps we worked with in order to visualize the data. The separation of the datasets was then created by extracting what we wanted to visualize on the map. For example, if we wanted to separate the monasteries based on seismic class, we visualized which monasteries are in a specific seismic zone. We made this separation not only for the seismic attributes, but for other attributes as well. 

Statistical Analysis:
	The data set was used to calculate different statistics depending on the field (for example, simple statistics were calculated to evaluate how many Null (or missing) values are found within a given field). 
	The installation of various libraries allowed for the creation of different types of maps using R studio. In order to create these maps, a get_map function had to be used so that we could specify which region we wanted to work with. For the purpose of this project, the region selected was Sicily. This enabled us to have a base map to work with. The beginning stages for code necessitated that we installed various packages in order to perform different functions on the dataset. We then began to write in clustering functions to group different monasteries based on seismic classification to determine whether any clustering occurred. 
	What we also did with these data is separate them depending on different attributes. For example, we created heat maps which show which areas have higher seismic classification values and we calculated which areas had more dedications than other areas. With the code, we were able to create chloropleth maps on the province level. Using GIS, we were able to separate the data at the municipal level. The problem with separating the maps at the municipal level is that it becomes messy. Although it is more accurate to separate different attributes based on the municipal level, it is not as visually intelligible as separating them at the province level.  
	The other interesting thing we did with the code is create an R shiny app which is interactive for the use of the different types of visualization that can be performed. It is convenient because the tab function allows us to visualize the datasets in different tabs. 
