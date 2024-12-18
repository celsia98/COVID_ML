# COVID_ML

COVID-19 Data Analysis and Mortality Prediction
Introduction
This project conducts an in-depth analysis of COVID-19 data to understand trends in case confirmations and fatalities, with a specific focus on mortality prediction using various machine learning algorithms. Utilizing data from Google Cloud's BigQuery, the script fetches a comprehensive dataset to explore pandemic dynamics over time and across different regions. The primary goal is to determine which predictive models most accurately estimate mortality rates based on available data, including confirmed cases, deaths, and administered vaccines.

Objectives
Data Extraction: Retrieve COVID-19 related data from Google Cloud BigQuery.
Data Cleaning and Transformation: Process and refine the data to prepare it for analysis.
Exploratory Data Analysis (EDA): Conduct initial investigations on the data to discover patterns, spot anomalies, and check assumptions with the help of summary statistics and graphical representations.
Model Development: Develop multiple machine learning models to predict mortality rates.
Model Comparison: Evaluate and compare the effectiveness of each model in predicting outcomes.
Visualization: Generate visual representations of data and predictions to better understand underlying trends.
Data Procurement
Data for this analysis is sourced from the Google Cloud BigQuery using:

BigQuery API: For structured querying and retrieval of data.
JSON Authentication File: Ensures secure access to BigQuery services.
Google Colab Integration: Provides a powerful and interactive environment for executing complex queries and storing intermediate results.
Data Structure
The dataset includes the following key columns:

date: The data collection date.
country_code: ISO code for the country.
location_key: Specific location identifier.
new_confirmed: Daily new confirmed COVID-19 cases.
new_deceased: Daily new COVID-19 related deaths.
cumulative_vaccine_doses_administered: Total vaccine doses administered until the date.
Algorithms Used
The project leverages several predictive models to estimate mortality rates:

Linear Regression
Gradient Boosted Trees
Random Forest
Elastic Net
Decision Tree Regressor
Lasso Regression
Support Vector Machines (SVM)
Key Features
Data Extraction and Cleaning: Efficient retrieval and preprocessing of large-scale data from BigQuery.
Exploratory Data Analysis (EDA): Utilizes statistical graphs and data-driven insights to understand the spread and impact of the virus.
Predictive Modeling: Implements and tunes several algorithms to forecast mortality based on observed data.
Model Comparison: Uses metrics such as R² and RMSE to assess model performances.
Visualization: Creates dynamic visualizations that illustrate both the historical trends and predictive analytics results.
Frameworks and Technologies Used
Google Colab: For executing Python notebooks with an integrated environment.
PySpark: Manages large data transformations and analysis.
Google BigQuery: Handles large-scale data storage and SQL queries.
Pandas: Facilitates data manipulation and analysis.
Matplotlib & Seaborn: Provides tools for creating a variety of visualizations.
Scikit-learn: Offers efficient tools for data mining and analysis.
Implementation Steps
Setup Environment: Configuring access to Google Cloud and initializing the analysis environment in Colab.
Data Extraction and Cleaning: Automated scripts to fetch and clean data.
Exploratory Data Analysis: Visual and statistical analysis to understand data characteristics.
Model Training and Evaluation: Systematic training and validation of predictive models.
Visualization and Insights: Development of insightful visualizations and interpretation of model predictions.
Model Performance Metrics
Performance of each model is evaluated using:

R² (Coefficient of Determination): Reflects the proportion of variance in the dependent variable predictable from the independent variables.
RMSE (Root Mean Squared Error): Measures the average magnitude of the prediction errors.
