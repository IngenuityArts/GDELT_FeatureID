# GDELT_FeatureID
This is a refinement of the GDELT FeatureID .txt file to make it more useable for apps and dashboards. The original GDELT lookup file is found here: http://data.gdeltproject.org/blog/2018-featureidcommonnames-crosswalk-may2018update/featureidcommonnames-crosswalk-may2018update.csv

The problem is that the "location" column has three comma separated values in the same column. This causes some issues for things like RShiny apps and others that aren't sure what to do with that format. This is how the original .csv file looks:
"featureid", "location", "lat", "long"
Under the "location" for example, you would see: "Aabo, Midtjylland, Denmark"

I split that column into  three: "location", "prov", "country" to make it easier to access and use. 
Now I have "location" Aabo, "prov" Midtjylland, "country" Denmark.

I have posted this new file as both a .csv and a .txt (tab delimted). 
