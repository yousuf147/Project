Project Overview
This project simulates a real-world data science workflow centered around predicting real estate prices. It leverages data from two sources and applies end-to-end data processing and modeling techniques. The main goals are:

Gathering property data from two distinct APIs.

Cleaning, transforming, and merging the datasets.

Developing and evaluating machine learning models for property price prediction.

Deploying both the data preprocessing and prediction logic as standalone API endpoints.

All project components and deliverables are available in this GitHub repository.

 Data Sources
The project uses the following APIs for data collection:

API 1 – ATTOM Data API
https://www.attomdata.com/solutions/property-data-api/

API 2 – Simulated Local API
A custom FastAPI service that generates synthetic property data. The implementation details are included in the repository.

Data Collection & Cleaning Process
Retrieved property data in JSON format from the ATTOM API.

Generated over 500 rows of synthetic property data using the FastAPI simulator.

Combined both datasets into a single DataFrame.

Applied the following data cleaning steps:

Removed duplicate and null entries.

Standardized and converted inconsistent data types.

Addressed missing fields and columns.

Eliminated irrelevant or redundant attributes.

 Modeling Strategy
Three machine learning models were trained and compared:

Decision Tree Regressor

Random Forest Regressor

XGBoost Regressor

 Best Performing Model:
The Random Forest Regressor achieved the highest accuracy and outperformed the others in evaluation metrics. (Detailed results are available in the code notebooks.)

 API Deployment
The data preprocessing pipeline is deployed as a FastAPI endpoint.

The final predictive model is also served via FastAPI for real-time property price inference.
