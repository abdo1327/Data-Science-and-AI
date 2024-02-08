# SpaceX Falcon 9 Launch Analysis

## Introduction
This repository contains the key findings and methodologies from the capstone project for (IBM Data science Professional Certificate)  aimed at predicting the successful landing of the Falcon 9 first stage for SpaceX launches. The analysis encompasses trends, observations, and predictions related to various aspects of SpaceX launching dates, including launch sites, success rates, and classification for the success of the landing and associated landing costs.

## Objective
The primary objective of this capstone project was to forecast the successful landing of the Falcon 9 first stage. By predicting landing success, we aimed to estimate launch costs, which are crucial for competitors bidding against SpaceX. The project involved collecting and formatting data from an API provided by SpaceX, performing exploratory data analysis (EDA) using visualization techniques, and conducting predictive analysis using classification models.

## Methodology
### Data Collection
- Identified relevant data sources, including SpaceX's API, to collect real information on Falcon 9 launches, including launch outcomes and landing status.
- Accessed the data sources through appropriate means, such as obtaining API keys.
- Extracted the required data using methods such as calling APIs.

### Data Wrangling
- Loaded the SpaceX dataset using pandas.
- Handled missing values by calculating their percentage.
- Inspected data types and identified numerical and categorical columns.
- Created labels for successful and unsuccessful landings based on mission outcomes.
- Exported the processed dataset with labels for further analysis.

### Exploratory Data Analysis (EDA)
- Utilized visualization techniques to explore SpaceX launch data, understanding launch outcomes, success rates across sites, and relationships between payload mass, booster versions, and success.
- Employed SQL queries to extract specific insights such as unique launch site names, payload mass statistics, and the date of the first successful landing outcome.
### Build a Dashboard with Plotly Dash 
"The Plotly Dash dashboard for SpaceX launch data includes:
Launch Site Drop-down: Users choose a launch site.
Success Pie Chart: Shows success/failure distribution based on the selected site.
Payload Range Slider: Filters launches by payload mass.
Success Payload Scatter Chart: Displays payload mass vs. success/failure, color-coded by booster version.
These features enable users to:
Identify the site with the most successful launches and highest success rate.
Analyze how payload mass affects launch success.
Determine success rates for different payload ranges and booster versions."
### Predictive Analysis (Classification)
- Explored the data to understand its features.
- Standardized all features to ensure they had the same scale.
- Split the data into training and testing sets.
- Tested various models including Logistic Regression, SVM, Decision Tree, and KNN.
- Tuned model parameters using GridSearchCV.
- Evaluated each model's accuracy on the test data and selected the Decision Tree model as the final model due to its superior performance.

## Results
### Exploratory Data Analysis (EDA) Results
- Explored SpaceX launch data to understand launch outcomes, success rates across sites, and relationships between payload mass, booster versions, and success.

### Predictive Analysis Results
- Trained models to predict launch success based on factors like payload mass, site, and booster version.
- Selected the Decision Tree model as the best-performing model for predicting Falcon 9 first stage landing.

## Files Included
- `README.md`: This file providing an overview of the project, methodology, and results.
-  `1_Collecting_the_data`:Jupyter Notebook containing the data Collectiong  process
-  `2_Web_scraping_Falcon_9_and_Falcon_Heavy_`:Jupyter Notebook containing the data Collectiong using Web scraping
-  `3_Data_wrangling.ipynb`: Jupyter Notebook containing the data wrangling process.
-  `4.ipynb`: Jupyter Notebook with the exploratory data analysis and vizs.
-  `5_SQL_&_sqllite`:upyter Notebook containing the connection to SQL database using sqlite
-  `6_Launch_Sites_Locations_Analysis_with_Folium`: Jupyter Notebook mapping the lunch locations using Folium lib  
-  `7_Machine_Learning_Prediction.ipynb`: Jupyter Notebook detailing the predictive analysis using classification models and compar thier preformnce.
-  `spacex_dash_app.py`: python code to create interactive dashboard uisng Dash and ploty.
-  `spacex_launch_dash.csv`: the dataset uesd by `spacex_dash_app.py`
-  `Dashboard 1`: image for the interactive dashboard  visualization and analysis.
-  `Dashboard 2`: another image for the interactive dashboard  visualization and analysis.
- `requirements.txt`: File listing all Python packages required to reproduce the analysis.

## Conclusion
This capstone project successfully explored SpaceX launch data, identified trends, and built a predictive model for forecasting Falcon 9 first stage landing success. The findings and methodologies presented here provide valuable insights for stakeholders interested in understanding and predicting SpaceX launch outcomes.


