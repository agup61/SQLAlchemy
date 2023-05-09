# SQLAlchemy

**Requirements**

Download the 2 CSV files and sqlite file provided in the Resources folder.
Python v3.10.9
Install SQL Alchemy
Install Numpy
Install Matplotlib
Install Datetime
Install Pandas

**1: Analysis and explore the climate data**

In this segment, we undertook a comprehensive analysis of the climate data by leveraging the programming tools Python, Pandas, and Matplotlib. Our team executed the following tasks:

1. Conducted an in-depth analysis of precipitation and station data.
2. For the precipitation analysis:
3. Identified the most recent date recorded in the dataset.
4. Utilized this date to obtain the preceding 12 months' precipitation data by running a query on the previous year's data.
5. Transferred the obtained results into a Pandas DataFrame.
6. Sorted the values in the DataFrame based on the "date" field.
7. Generated a visual representation of the data using the DataFrame plot method.
8. Determined summary statistics for the precipitation data utilizing Pandas.
9. Created a query to establish the total number of stations in the dataset.
10. Developed a query to pinpoint the stations with the highest activity levels.
11. Using the station with the most activity, determined the highest, lowest, and average temperatures recorded.
12. Designed a query to gather the temperature observation (TOBS) data from the previous 12 months.
13. Filtered the results based on the station with the highest number of observations.
14. Retrieved the temperature observation (TOBS) data for the preceding 12 months for that station.
15. Visualized the results as a histogram with 12 bins.

**2: Design your climate app

In this section, our team created a Flask API that was built around the queries developed in Part 1. To accomplish this, we designed the following routes:

1. Home Page: This serves as the starting point for the API.
2. List of Available Routes: This provides a list of all the available routes that users can access.
3. JSON List: The following routes return a JSON list:

- /api/v1.0/precipitation
- /api/v1.0/stations
- /api/v1.0/tobs
4. Route /api/v1.0/: This route provides the minimum temperature, average temperature, and maximum temperature for a specified start date.
5. Route /api/v1.0// : This route provides the minimum temperature, average temperature, and maximum temperature for a specified start-end range.

Both responses for routes 4 and 5 return a list of the minimum temperature, average temperature, and maximum temperature for the specified start or start-end range.

**References**

Menne, M.J., I. Durre, R.S. Vose, B.E. Gleason, and T.G. Houston, 2012: An overview of the Global Historical Climatology Network-Daily Database. Journal of Atmospheric and Oceanic Technology, 29, 897-910, https://doi.org/10.1175/JTECH-D-11-00103.1Links to an external site., measurements converted to metric in Pandas.
