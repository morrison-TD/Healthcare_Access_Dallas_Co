
# Healthcare Facility Accessiblity
----------------------------
The Goal of the Healthcare Accessiblity project was to exmine the access of healthcare facilities in Dallas County by income level.

![Multi-layer Google Map: Poverty Heatmap, Hospitals and Clinics](/images/HospitalsandUCHeatMap.png)



## Data
----------
* US Census Data was used to grab Poverty Ratings, Income Levels and Zipcodes. (Resources/DallasCensusData.csv)

* MediCare data was used to examine MediCare certified https://www.medicare.gov/hospitalcompare/search.html? hospitals within the county (needed a metric from suitable care facilities)

* Google's Geocoding was used to return the locations of Google registered "Urgent Care", non-emergency facilities within Dallas County. These facilites are not federally rated. (Resources/ClinicMasterComplete.csv)


## Cleaning the Data
--------------
First we cleaned US Census Data to isolate the zipcodes, we then pushed those zipcodes to Google Geocode to extract the zipcodes within Dallas County.  The Census data included a Poverty Index Rating, we used this index to create a Google Heatmap to show the impoverished areas.

![Dallas Poverty Heat Map](/images/PovertyHeatMap.png)


We then pulled MediCare Hospital data to return a list of Hospitals registered with MediCare.gov. Using the Google parameters for Dallas County, we returned a list of hospitals within Dallas County. Map them with Google.

![Dallas County Hospital Map](/images/HospitalMap.png)


Finally, we requested all the registered "urgent care" clinics within the Dallas County area, using the Google Geocode feature. 


![Dallas County Urgent Care Clinics](/images/UrgentCaresDallasCounty.png)

# Findings
-----------

Based on the data we found that hospitals were more likely to be located outside of income areas:

![Dallas County Hospital Bar Chart](/images/HospitalsbyIncomeLevelBar.png)

Urgent care clinics were also more likely to be located outside of low income areas:

![Dallas County Urgent Care Bar Chart](/images/UrgentCarebyIncomeLevelBar.png)







