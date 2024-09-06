# Data Dictionary for Hourly Arctic Rain on Snow Database

This data dictionary describes hourly files in the Arctic Rain on Snow Database.

Add processing stream

Hourly files contain aggregated sub-hourly records for stations.

From https://atlan.com/what-is-a-data-dictionary/#what-is-a-data-dictionary

A listing of data objects (names and definitions)
Detailed properties of data elements (data type, size, nullability, optionality, indexes)
Entity-relationship (ER) and other system-level diagrams
Reference data (classification and descriptive domains)
Missing data and quality-indicator codes
Business rules, such as for validation of a schema or data quality
Additionally, the data dictionary should also include information on:

Data source (data warehouse, data lakes, databases, applications)
Date and time when the property was created or changed
Descriptive statistics that go beyond missing values, such as min-max values and histogram distribution
Owners and editors of data sets that contain these variables
SQL queries attached to the data asset
Social metadata associated with each data asset - stored as tags, notes, and chat transcripts


object, data-type, units, missing-data, source, min, max, description
datetime, datetime, -, -, clean, -, , "datetime for observation hour"
station, string, -, -, clean, None, , "four letter station identifier, metadata/aross.asos_station.metadata.csv
t2m, float, celsius, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "air temperature at 2 meters above ground surface"
d2m, float, celsius, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "dew point temperature of air at 2 meters above ground surface"
relh, float, percent, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "relative humidity of air at 2 meters above ground surface"
mslp, float, hPa, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "mean sea level pressure"
psurf, float, hPa, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "surface pressure"
p01i, float, mm, , "arithmetic mean of t2m values in clean for hour preceding", ?, ?, "one hour precipitation for the period from the observation time to the time of the previous hourly precipitation reset"
UP, bool, , "True if UP observed in period from time of observation to time of previous observation", True, False, "unknown precipitation reported in METAR" 
RA, bool, , "True if RA observed in period from time of observation to time of previous observation", True, False, "liquid precipitation (rain) reported in METAR"
FZRA, bool, , "True if FZRA observed in period from time of observation to time of previous observation", True, False, "freezing precipitation reported in METAR"
SOLID, bool, , "True if SN observed in period from time of observation to time of previous observation", True, False, "solid precipitation reported in METAR"
wspd, float, m/s, "magnitude of mean of wind vector from time of observation to time of previous observation", ?, ?, "wind speed at approximately 10 m above ground surface"
drct, float, degree, "direction from north of wind vector from time of observation to time of previous observation", ?, ?, "wind direction at approximately 10 m above ground surface"
