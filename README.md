# CAPSTONE DEMO README

### Describe your project (big idea)
Uber and Lyft drivers can gain from data-driven insights to increase their earnings and increase their efficiency during their driving sessions.

### Describe your goal
To provide recommendations as a resource for Uber and Lyft drivers, helping them implementing their knowledge of the markets and cities where they drive, along with their understanding of surge pricing (surge multipliers), to predict increases in driver earnings and enhance efficiency during driving sessions.

### Describe your data
The datasets utilized thus far are named "cab_rides.csv" and "weather.csv". "Cab_rides.csv" contains 693071 rows and 11 columns of data originally utilzed for predicting rideshare service demand in Boston, MA and its surrounding areas over the span of about 1 week in November, 2018. The "weather.csv" dataset contains 6276 rows and 8 columns of data with variables such as 'temperature', 'precipitation', 'air pressure', 'wind', 'humidity', and others. The two datasets combined are purposed to support a more robust prediction, relative to just a singular dataset, for the demand of Uber and Lyft trips.     

### Describe your work (models, analysis, EDA, etc.)
EDA is still in an iterative process, however, interesting figures have been found, e.g., 56% of trips recorded during the test were via the Uber platform while 44% were via Lyft. Another finding showed that the most ordered 'Product_ID' (rideshare service type) was the 'UberXL' vehicles. As for the analysis phase, the Moving Average technique looks to be a likely choice. It could be initially used as a simple moving average for the 'Surge_Multiplier' variable, which is the primary field of interest for this capstone. Then, correlations could be drawn between a simple moving average and various weather variables, such as 'temperature' and 'rain,' to identify the effect of weather on surge pricing. In the modeling phase, a weighted moving average could be useful as additional data is incorporated into the model in later stages. However, a better understanding of ML models ought to influence the decision on techniques utilized for this stage.  

### Describe your results
Pending descriptive results as eda, analysis, and modeling is underway.

### Party!
