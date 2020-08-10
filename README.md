## BayWheels-Project

I wanted to visualize how bike share traffic in SF changed around COVID-19. Using publicly available data from Lyft's BayWheels program, I mapped the number of rides initiated by zip code by week for 2020. 

### Data Import
- Pull in CSVs for January - June 2020 into One DataFrame
- Import Jan - Mar files into DataFrame
- Map Apr - Jun data to Q1 format into DataFrame
- Concatenate the 2 Dataframes (inner)

### Data Cleaning
- Update 24 records starting at 16th St Fleet Depot from (0,0) to NaN. 
- Remove partial weeks at beginning/end of data set
- Adding additional date fields (first day of week, week number)
- Creating binary COVID variable (<3/16/20 --> COVID=0 ; >=3/16/20 --> COVID=1)

### Create GeoPanda
- Transform start coordinates into coordinates geometry format
- Create GeoPanda

### Map Rides to Zip Codes
- Import Bay Area Zip Shape File
- sjoin with DataFrame
- Restrict to SF Zip Codes

### Basic Information on Behavior Pre/Post COVID-19
- Top Stations
- # of Rides by Week
- # of Rides by Day of Week
- Rides by Week by Zip Code

### GIF Creation
- Create images of rides by week by zip code
- Create GIF in CL using ImageMagick


### Sources¶
This information, particularly the tutorials and guides on Medium, were instrumental in this project

Medium Articles
- Importing CSVs: https://medium.com/@kadek/elegantly-reading-multiple-csvs-into-pandas-e1a76843b688
- Time lapse display: https://medium.com/@tyreus/visualizing-the-spread-of-the-2019-coronavirus-with-python-7e63230f9505
- GeoPandas Plotting: https://towardsdatascience.com/geopandas-101-plot-any-data-with-a-latitude-and-longitude-on-a-map-98e01944b972

Primary Sources
- Bike Data: https://s3.amazonaws.com/baywheels-data/index.html
- Shape Files: https://geodata.lib.berkeley.edu/?bbox=-127.749023+29.036961+-112.412109+45.675482&f%5Bdc_format_s%5D%5B%5D=Shapefile&f%5Bdct_spatial_sm%5D%5B%5D=San+Francisco+Bay+Area+%28Calif.%29&per_page=10

Formal Documentation
- Pandas: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
- GeoPanda Documentation: https://geopandas.org/reference.html
- Matplotlib Colors: https://matplotlib.org/3.1.0/gallery/color/named_colors.html

Historical Context
- Bay Wheels Feb Price Increase: https://mashable.com/article/lyft-bay-wheels-ebike-price-increase/
- COVID Timeline in Bay Area: https://abc7news.com/timeline-of-coronavirus-us-coronvirus-bay-area-sf/6047519/
- Remote Work Timeline: https://www.sfgate.com/bayarea/article/coronavirus-Bay-Area-companies-work-from-home-news-15111144.php
