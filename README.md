## BayWheels-Project


### Goals
I wanted to visualize how bike share traffic in SF changed with COVID-19. Using publicly available data from Lyft's BayWheels program, I mapped the number of rides initiated by zip code by week for 2020. 

Research question : How has COVID-19 changed BayWheels user behavior?

### Write Up
Check out this wiki for [my analysis](https://github.com/kailinkoch/baywheels-project/wiki/Insights-from-baywheels-project)


### Steps
- Pulled CSVs from Jan-Jun 2020 into Dataframe
- Renamed the columns names for Apr-Jun, because they changed. May also had an additional column. 
- Removed the partial weeks at the beginning of January and end of June to do a comparison of full weeks only
- Removed 24 records with (0,0) starting point
- Created a COVID variable that started on 3/17/2020
- Create GeoPanda with Geometry points
- Map to SF Zips, restrict to SF Zips only (not full Bay Area)
- Gather basic information on pre/post COVID-19 and create charts
- Map top stations
- Map rides by week by zip code
- Create GIF

### Progress
- Data Analysis complete
- Created GIF and Charts
- To Complete: Automate Ingestion of CSVs
- To Complete: Re-factor Jupyter Notebook into Pycharm

### Data Sources
- [Bike Data](https://s3.amazonaws.com/baywheels-data/index.html)
- [Shape Files](https://geodata.lib.berkeley.edu/?bbox=-127.749023+29.036961+-112.412109+45.675482&f%5Bdc_format_s%5D%5B%5D=Shapefile&f%5Bdct_spatial_sm%5D%5B%5D=San+Francisco+Bay+Area+%28Calif.%29&per_page=10)

### Other Sources 
This information, particularly the tutorials and guides on Medium, were instrumental in this project

Approach
- [Time lapse GIF](https://medium.com/@tyreus/visualizing-the-spread-of-the-2019-coronavirus-with-python-7e63230f9505)
- [Importing CSVs](https://medium.com/@kadek/elegantly-reading-multiple-csvs-into-pandas-e1a76843b688)
- [GeoPandas Plotting](https://towardsdatascience.com/geopandas-101-plot-any-data-with-a-latitude-and-longitude-on-a-map-98e01944b972)

Historical Context
- [Bay Wheels Feb Price Increase](https://mashable.com/article/lyft-bay-wheels-ebike-price-increase/)
- [COVID Timeline in Bay Area](https://abc7news.com/timeline-of-coronavirus-us-coronvirus-bay-area-sf/6047519/)
- [Remote Work Timeline](https://www.sfgate.com/bayarea/article/coronavirus-Bay-Area-companies-work-from-home-news-15111144.php)
