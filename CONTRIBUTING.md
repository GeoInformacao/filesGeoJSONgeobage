## Become a filesGeoJSONgeobage contributor:

If you would like to contribute to filesGeoJSONgeobage, the first thing to do is open an [issue](https://github.com/GeoInformacao/geobage/issues) on Github with your suggestion of a function or dataset you would like to see in the package. Keep in mind that, as a rule, the package includes only geospatial datasets with national spatial coverage over the municipality of Bagé - RS and that are created/managed by government institutions and are publicly available.

Adding each dataset to the geobage follows a three-step process as follows:

### Step 1. Data preparation

In the first step, the contributor should write an `R` script that will prepare the raw original data set to be used in geobage. This script should (1) download the raw data from the original website source, (2) rename column names following a simple spelling convention*, (3) ensure the data uses spatial projection EPSG 4674, (4) ensure every string column is `as.character` with UTF-8 encoding, (5) fix eventual topology issues in the data, and (6) save the data in `.geojson` format. (7) The file name must be in all caps.

This script can use any `R` package, but it needs to be 100% reproducible.

### Step 2. Data validation and upload

Once the prep_ script is ready, the team will test the script and validate the data output. If everything works fine, the team will upload the data to our servers so it will become available for download. If everything works fine, the contributor can open a pull request and start the celebration. We will update our documentation to add your name to our contributors team.

Spelling conventions: Names should be lower case, short, use underscore when necessary, use English American spelling. Please have a look at the columns names and don't hesitate to contact if you have any question.
