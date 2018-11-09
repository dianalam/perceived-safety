# Perceptions of Urban Perception
A project that uses machine learning to determine the socioeconomic impacts of perceived safety in urban environments.

Our perceptions of the urban landscape--sidewalks, buildings, roads--can differ wildly from the actual experience of neighborhoods. This project investigates the differences between perception and reality in terms of safety/crime in New York City neighborhoods. Which neighborhoods are perceived as more dangerous or safer than they actually are? What are the socioeconomic and physical features that characterize these neighborhoods? Answering these questions can help urban dwellers and policymakers understand the way urban perception is related to livability and guide future planning initiatives.

For more information on the project, see [my blog post][blog].

For the neighborhood explorer tool, see [this link][explorer tool].

## In this repo

* `app/`: Contains code and artifacts for the interactive neighborhood explorer tool.
* `reverse-geocode.ipynb`: Jupyter notebook containing code to reverse geolocate crime, perceived safety, and other select socioeconomic/physical data. Converts from longitude and latitude pairs into census tracts.
* `safety-analysis-final.ipynb`: Jupyter notebook containing code to develop a custom scoring mechanism to categorize neighborhoods as safer than perceived, neutral, or more dangerous than perceived. Also contains code to build models to predict the category of each neighborhood based on its socioeconomic and physical features.
* `neighborhood-finder-app.ipynb`: Jupyter notebook containing code to generate data for app.
* `archive/`: Contains scratchwork documenting the evolution of the project.

## Data Sources
* [MIT Media Lab Streetscore]: Perceived safety data.
* [NYPD Citywide Major Felony Offenses]: Crime data.
* [U.S. Census & American Community Survey]: Various demographic/socioeconomic datasets, including:
	* Educational attainment in persons 25 years and older
	* Employment
	* Housing type
	* Age and sex
	* Household income
	* Median home value & rent
	* Median year house was built
	* Occupied and vacant units
	* Population
	* Race 
* [NYC 311 Complaints]
* [NYC Department of City Planning]: Land use data, including:
	* Property assessed value
	* Land use 
	* Building age
	* Built height
* [NYC Subway Stations]: Transit access

[blog]: https://dianalam.com/2016/04/04/urban-perception.html
[explorer tool]: http://dianalam.github.io/perceptions/map.html
[MIT Media Lab Streetscore]: http://streetscore.media.mit.edu/data.html
[NYPD Citywide Major Felony Offenses]: https://www1.nyc.gov/site/nypd/stats/crime-statistics/historical.page
[NYC 311 Complaints]: https://data.cityofnewyork.us/Social-Services/311-Complaint-Types/h4xh-jcuz
[NYC Subway Stations]: https://data.cityofnewyork.us/Transportation/Subway-Stations/arq3-7z49
[U.S. Census & American Community Survey]: https://factfinder.census.gov/faces/nav/jsf/pages/index.xhtml?
[NYC Department of City Planning]: https://www1.nyc.gov/site/planning/data-maps/open-data.page


