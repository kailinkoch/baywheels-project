## BayWheels-Project

## Goals
I wanted to visualize how bike share traffic in SF changed with COVID-19. Using publicly available data from Lyft's BayWheels program, I mapped the number of rides initiated by zip code by week for 2020. 

Research question : How has BayWheels bike ride behavior changed as a result of COVID-19?

### Steps
- Pull CSVs from Jan-Jun 2020 into Dataframe
- Clean up records (remove partial weeks, create COVID variable etc)
- Create GeoPanda with Geometry points
- Map to SF Zips, restrict to SF 
- Gather basic information on pre/post COVID-19 and display as charts
- Map rides by week by zip code
- Create GIF

### Progress
- Data Analysis complete
- Created GIF and Charts
- To Complete: Automate Ingestion of CSVs
- To Complete: Final de-duping checks for data between months

### Data Sources
- Bike Data: https://s3.amazonaws.com/baywheels-data/index.html
- Shape Files: https://geodata.lib.berkeley.edu/?bbox=-127.749023+29.036961+-112.412109+45.675482&f%5Bdc_format_s%5D%5B%5D=Shapefile&f%5Bdct_spatial_sm%5D%5B%5D=San+Francisco+Bay+Area+%28Calif.%29&per_page=10

### Other Sources 
This information, particularly the tutorials and guides on Medium, were instrumental in this project

Approach
- Importing CSVs: https://medium.com/@kadek/elegantly-reading-multiple-csvs-into-pandas-e1a76843b688
- Time lapse display: https://medium.com/@tyreus/visualizing-the-spread-of-the-2019-coronavirus-with-python-7e63230f9505
- GeoPandas Plotting: https://towardsdatascience.com/geopandas-101-plot-any-data-with-a-latitude-and-longitude-on-a-map-98e01944b972

Historical Context
- Bay Wheels Feb Price Increase: https://mashable.com/article/lyft-bay-wheels-ebike-price-increase/
- COVID Timeline in Bay Area: https://abc7news.com/timeline-of-coronavirus-us-coronvirus-bay-area-sf/6047519/
- Remote Work Timeline: https://www.sfgate.com/bayarea/article/coronavirus-Bay-Area-companies-work-from-home-news-15111144.php
