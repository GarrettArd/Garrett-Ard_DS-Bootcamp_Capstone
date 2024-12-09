# CAPSTONE DEMO README

### <ins>Describe Your Project (big idea)</ins>
Uber and Lyft drivers can gain from data-driven insights to increase their earnings and increase their efficiency during their driving sessions.

### <ins>Describe Your Goal</ins>
To provide recommendations as a resource for Uber and Lyft drivers, helping them implementing their knowledge of the markets and cities where they drive, along with their understanding of surge pricing (surge multipliers), to predict increases in driver earnings and enhance efficiency during driving sessions.

### <ins>Describe Your Data (data source included)</ins>
The datasets utilized thus far are named "cab_rides.csv" and "weather.csv". "Cab_rides.csv" contains 693071 rows and 11 columns of data originally utilzed for predicting rideshare service demand in Boston, MA and its surrounding areas over the span of a couple months in Septmeber to December 2018. The "weather.csv" dataset contains 6276 rows and 8 columns of data with variables such as 'temperature', 'precipitation', 'air pressure', 'wind', 'humidity', and others. The two datasets combined are purposed to support a more robust prediction, relative to just a singular dataset, for the demand of Uber and Lyft trips. The two datasets used for this capstone can be found here: https://www.kaggle.com/datasets/ravi72munde/uber-lyft-cab-prices/data?select=weather.csv.      

### <ins>Describe Your Work (models, analysis, EDA, etc.)</ins>
EDA is still in an iterative process, however, interesting figures have been found, e.g., 56% of trips recorded during the test were via the Uber platform while 44% were via Lyft. Another finding showed that the most ordered 'Product_ID' (rideshare service type) was the 'UberXL' vehicles. As for the analysis phase, I still intend to do a Time Series analysis along with showing a Moving Average of the `surge_multiplier`, however, at the current point in time, I have gone with a multiclass classification, Logistic Regression model. The time series analysis could be initially used as a simple moving average for the 'Surge_Multiplier' variable, which is the primary field of interest for this capstone. Then, correlations could be drawn between a simple moving average and various weather variables, such as 'temperature', 'rain,' and 'wind', for example, to identify the effect of weather on surge pricing (in effect, the surge_multiplier applied to price). As for my logistic regression model, I only selected the destination, source, and time_stamp variables for my predictors based on domain knowledge considering these variables would be the only I felt would have real impact on the surge_multiplier variable. Another iteration of the logistic regression model is intended to be done with weather conditions and their predictive impact on the `surge_category_multiplier`. In the modeling phase, a weighted moving average could be useful as additional data is incorporated into the model in later stages. However, a better understanding of ML models ought to influence the decision on techniques utilized for this stage.

### <ins>Code Structure</ins>
The code follows a structure of five main steps that correlate to the main processes followed for the project. These consist of: 1) Data loading and cleaning, 2) Exploratory Data Analysis (EDA), 3) Pre-processing, 4) Modelling, 5) Findings. The data for this project is decently clean, so, step 1 and the code involved is relatively brief. Much effort has gone into the EDA step as this phase serves as an important foundation to the following phases/steps of the project. Much of the code is distributions of numerical and some categorical data. The purpose of EDA is to gain further understanding of the data and to help better visualize the question of interest so the reader can comfortably understand where the process is going as the processes move into the 3rd step. 

### <ins>Future Work</ins> 
The 3rd step is Pre-processing, which is manipulating the data to prepare it for modelling. The preprocessing for Logistic Regression concsitst of separating the variables, applying the train_test_split from sklearn, and initalizing, fitting, and finally training the model. Once trained, the data is predicted upon yielding accuracy, precision, recall scores and other metrics (typically provided by sklearn). As mentioned, I am in process of solidifying the time series analysis model that I plan to use and that I've mentioned in the previous section. This was an area I needed to revisit and refresh my understanding on before confidently implementing into the capstone. Once the code related to Time Series is finalized, I will update this section in this readme.md to more accurately describe the code that phase of the project for this section. Naturally, the code and code structure for step 4) and step 5) is pending as project develops. 

### <ins>Acknowledgements/References</ins>
I want to acknowledge the support and guidance from my educators at BrainStation, especially Laura Cornejo Paulino and Steven Savchik, as well as Borna Ghotbi, for #1, their teachings on the topics that have contributed to this project. Laura and Steven have given awesome feedback and direction to this project and #2 influenced its development in many ways from areas such as this very readme.md file to even the stat and ml models chosen that would best fit this project. Big shoutout and thanks educator staff at BrainStation! 

### <ins>Describe Your Results</ins>
................................EDA has developed more from Sprint 1 to Sprint 2. Some notable items found were: the `time_stamp` column in the `cab_rides` dataset needed to be converted to datetime, as it initally was a long string of numbers that was representing milliseconds. This has been done and `time_stamp` is now able to be used for Time Series analysis. Another item noticed was that we're slightly more uber drivers than lyft. Somthing that could be further evaluated (and has been suggested to me) is to see if there is a shortage of lyft drivers and what effect that can have on the overall demand for a city/market. Regarding the `weather` dataset, I decided to spotlight three weather conditions that I thought most people would deem impactful in their decision to use Uber/Lyft and those are 'temp', 'rain', and 'wind'. Something noteworthy from these distributions was that the most rides completed were completed in about 40-41(°F) weather. Another surprising find from these three weather conditions was that the most rides completed were completed in ~9mph wind speed! As for the cab rides dataset, the highest number trips completed were ~1.5 miles in overall distance (source-destination). Another cab rides dataset insight was that the highest number of rides completed were priced at about ~$10 to the passenger. Some other distribtuions were done on the remaining weather conditions in the dataset beyond the three previously mentioned so be sure to check these out. Pending further descriptive results as eda, analysis, and modeling is underway.

### Party!
