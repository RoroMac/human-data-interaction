## HCDE410SP22 - Assignment A1

Adapted from # cdsw-2020 https://wiki.communitydata.science/Seattle_open_data

Assignments are taken from [Brock Craft's](https://github.com/brockcraft/hcde410sp22) and edited by me. This repo is protected under the MIT license.

### Datasets Used
The datasets come from the data.seattle.gov website underneath an open source and free-to-use policy. It's data use policy can be [summarized here](https://data.seattle.gov/stories/s/Data-Policy/6ukr-wvup/) and further [elaborated here](http://www.seattle.gov/Documents/Departments/SeattleGovPortals/CityServices/OpenDataPolicyV1.pdf). 


### Burke-Gilman.ipynb
Performs a basic data analysis about traffic along the trail from an API referencing a dataset from seatte.gov. The API retrieves information on both bikers and pedestrian traffic. Dictionaries and lists are used to determine the frequency of use across various time variables.

| Data Variable | Description |
|-----------| ------------|
| Date | Year-Month-Day-Hour-Minute-Second Format |
| Ped South | Number of pedestrians south bound at that time period |
| Ped North | Number of pedestrians north bound at that time period |
| Bike North | Number of bikers going north bound at that time period|
| Bike South | Number of bikers going south bound at that time period|

The bg_traffic_bike_ped_2019.csv is created in this file to avoid calling an API with to run each session. It contains the same variables as mentioned above.

### SODA_API_demo.ipynb
Examines various API calls using Seattle permit data. It creates a 1000_most_recent_residential_permits.csv containing 1000 containing the following information.

| Data Variable | Description |
| --------------| ----------- |
| Permit Number  | Unique ID of the building permit     |
| Description   | Description of the changes being done |
| Building Type  | What kind of purpose does the building have (residential, institutional, or commercial)|
| Completed Date | When the building was finished.
