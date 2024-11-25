# CAPSTONE DEMO README

### Describe your project (big idea)
Uber and Lyft drivers can gain from data-driven insights to increase their earnings and increase their efficiency during their driving sessions.

### Describe your goal
To provide recommendations as a resource for Uber and Lyft drivers, helping them implementing their knowledge of the markets and cities where they drive, along with their understanding of surge pricing (surge multipliers), to predict increases in driver earnings and enhance efficiency during driving sessions.

### Describe your data (data source included)
The datasets utilized thus far are named "cab_rides.csv" and "weather.csv". "Cab_rides.csv" contains 693071 rows and 11 columns of data originally utilzed for predicting rideshare service demand in Boston, MA and its surrounding areas over the span of about 1 week in November, 2018. The "weather.csv" dataset contains 6276 rows and 8 columns of data with variables such as 'temperature', 'precipitation', 'air pressure', 'wind', 'humidity', and others. The two datasets combined are purposed to support a more robust prediction, relative to just a singular dataset, for the demand of Uber and Lyft trips. The two datasets used for this capstone can be found here: https://www.kaggle.com/datasets/ravi72munde/uber-lyft-cab-prices/data?select=weather.csv.      

### Describe your work (models, analysis, EDA, etc.)
EDA is still in an iterative process, however, interesting figures have been found, e.g., 56% of trips recorded during the test were via the Uber platform while 44% were via Lyft. Another finding showed that the most ordered 'Product_ID' (rideshare service type) was the 'UberXL' vehicles. As for the analysis phase, the Moving Average technique looks to be a likely choice. It could be initially used as a simple moving average for the 'Surge_Multiplier' variable, which is the primary field of interest for this capstone. Then, correlations could be drawn between a simple moving average and various weather variables, such as 'temperature', 'rain,' and 'wind', for example, to identify the effect of weather on surge pricing (in effect, the surge_multiplier applied to price). In the modeling phase, a weighted moving average could be useful as additional data is incorporated into the model in later stages. However, a better understanding of ML models ought to influence the decision on techniques utilized for this stage.

### <u>Code structure</u>
The code follows a structure of five main steps that correlate to the main processes followed for the project. These consist of: 1) Data loading and cleaning, 2) Exploratory Data Analysis (EDA), 3) Pre-processing, 4) Modelling, 5) Findings. The data for this project is decently clean, so, step 1 and the code involved is relatively brief. Much effort has gone into the EDA step as this phase serves as an important foundation to the following phases/steps of the project. Much of the code is distributions of numerical and some categorical data. The purpose of EDA is to gain further understanding of the data and to help better visualize the question of interest so the reader can comfortably understand where the process is going as the processes move into the 3rd step. 

### <u>Future work</u> 
The 3rd step is Pre-processing, which is manipulating the data to prepare it for modelling. Currently, I am in process of solidifying the time series analysis model that I plan to use and that I've mentioned in the previous section. This was an area I needed to revisit and refresh my understanding on before confidently implementing into the capstone. Once the code related to Time Series is finalized, I will update this section in this readme.md to more accurately describe the code that phase of the project for this section. Naturally, the code and code structure for step 4) and step 5) is pending as project develops. 

### <u>Acknowledgements/References</u>
I want to take a moment and a few sentences here to acknowledge the support and guidance from my educators at BrainStation, especially Laura Cornejo Paulino and Steven Savchik (as well as Borna Ghotbi) for #1 their teachings on the topics. Laura and Steven have given awesome feedback and direction to this project and influenced its development in many ways from areas such as this very readme.md file to even the stat and ml models chosen that would best fit this project. Big shoutout and thanks educator staff at BrainStation! **Definitely check out BrainStation if interested in developing your digital skills!

### <u>Describe your results</u>
Pending descriptive results as eda, analysis, and modeling is underway.

### Party!
