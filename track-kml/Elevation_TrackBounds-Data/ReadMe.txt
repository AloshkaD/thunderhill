All of Polysync and GPS data is contained inside myplaces.kml
GoogleEarth_Elevation.py runs and compares the elevation data from the polysync dataset to the google api.
to run this code: do the following:

1. Ensure you have simplejson, urllib, numpy, matplotlib, fastkml installed.
2. Get your Google elevation api key from here (Its free): https://developers.google.com/maps/documentation/elevation/get-api-key
3. Run the following from a python console:
>> import GoogleEarth_Elevation
>> GoogleEarth_Elevation.compareElevation(<<path_to_myplaces.kml>>, <<your_google_api_key_>>)

4. If you want to get the elevation data from Google maps for the track bounds:
>> import GoogleEarth_Elevation
>> gps_data = GoogleEarth_Elevation.getCompleteGPSdata(<<path_to_myplaces.kml>>, <<your_google_api_key_>>)

Plots are checked-in for reference.
