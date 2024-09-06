# Data Dictionary for `aross.asos_stations.metadata.csv`

This is a data dictionary for the aross.asos_stations.metadata.csv file.

The file is a comma separated value (csv) file containing station metadata from the Iowa State University
Environmental Mesonet (IEM) archive of Automated Surface Observing System (ASOS) stations.

https://mesonet.agron.iastate.edu/ASOS/



stid - three or four letter [A-Z] station identification code
station_name - Name of station location
latitude - latitude in decimal degrees
longitude - longitude in decimal degrees
elevation - elevation of station in meters above sea level
record_begins - Date that station archive begins
iem_network - IEM network identifier
state - US State
country - Country Code
climate_site
wfo - National Weather Service Weather Forecast Office
tzname - name of time zone
ncdc81 - 
ncei91 - 
ugc_county - 
ugc_zone - 
county - 
network - 
start_year - First year of record
end_year - Last year of record


# ncdc81 and ncei91 station identifier codes

from [readme.txt](https://www.ncei.noaa.gov/pub/data/ghcn/daily/readme.txt) of GHCN-Daily

>ID         is the station identification code.  Note that the first two
           characters denote the FIPS  country code, the third character 
           is a network code that identifies the station numbering system 
           used, and the remaining eight characters contain the actual 
           station ID. 

           See "ghcnd-countries.txt" for a complete list of country codes.
	   See "ghcnd-states.txt" for a list of state/province/territory codes.

           The network code  has the following five values:

           0 = unspecified (station identified by up to eight 
	       alphanumeric characters)
	   1 = Community Collaborative Rain, Hail,and Snow (CoCoRaHS)
	       based identification number.  To ensure consistency with
	       with GHCN Daily, all numbers in the original CoCoRaHS IDs
	       have been left-filled to make them all four digits long. 
	       In addition, the characters "-" and "_" have been removed 
	       to ensure that the IDs do not exceed 11 characters when 
	       preceded by "US1". For example, the CoCoRaHS ID 
	       "AZ-MR-156" becomes "US1AZMR0156" in GHCN-Daily
           C = U.S. Cooperative Network identification number (last six 
               characters of the GHCN-Daily ID)
	   E = Identification number used in the ECA&D non-blended
	       dataset
	   M = World Meteorological Organization ID (last five
	       characters of the GHCN-Daily ID)
	   N = Identification number used in data supplied by a 
	       National Meteorological or Hydrological Center
           P = "Pre-Coop" (an internal identifier assigned by NCEI for station
               records collected prior to the establishment of the U.S. Weather
               Bureau and their management of the U.S. Cooperative (Coop) 
               Observer Program
	   R = U.S. Interagency Remote Automatic Weather Station (RAWS)
	       identifier
	   S = U.S. Natural Resources Conservation Service SNOwpack
	       TELemtry (SNOTEL) station identifier
           W = WBAN identification number (last five characters of the 
               GHCN-Daily ID)

