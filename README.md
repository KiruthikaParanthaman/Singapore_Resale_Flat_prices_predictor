# Singapore Resale Flat Prices Predictor
**Problem Statement:**
Singapore Housing and Development Board(HDB) has dataset of resale flat transactions from 1990 to till date. Objective of this project is to to develop a machine learning model and develop a user-friendly web application that predicts the resale prices of flats in Singapore.This predictive model will be based on historical data of resale flat transactions, and it aims to assist both potential buyers and sellers in estimating the resale value of a flat.

**Tools and Technologies Used:** 
Python,Jupyter Notebook,Streamlit

**Model-Building Approach:**
Dataset from Singapore Housing Development Board was downloaded from 1990 to March-mid 2024. Datasets in csv format converted to dataframe and Exploratory Data Analysis was performed before merging all the datasets into single dataframe.Missing columns like 'Remaining Lease' was featured using available data of Transaction date and Lease Start date. Null values,outliers and datatype compatibility checked.After Datatype conversion datsets were merged. Based EDA, new column "Building_age_today" which specifies building age of Flats based on Lease commencement date was calculated.Columns with no useful information like "block" was dropped,followed by Label Encoding,Standardization,Model-building and deploy streamlit app. Complete EDA description could be accessed [here](https://github.com/KiruthikaParanthaman/Singapore_Resale_Flat_prices_predictor/blob/main/Project%20Singapore%20Resale%20Flat%20Price.ipynb)

Further analysis like Uni-variate, Bi-variate Analysis done which displayed some interesting relations. Pearson co-relation displayed high dependancy in some of the independant variables/predictor variables like Flat-type-Floor-sqm,Remaining lease- Building age days. Hence highly correlated variables was dropped to reduce noise and to increase accuracy.Standard Scaler was used to standardize the dataset, followed by splitting of data into Train, Validation and Test dataset. The prediction involves predicting continuous variable i.e., Resale price hence various regression model like Linear Regression nd tree based models like Decision Tree,Random Forest,Adaboost Regressor,XGboost Regressor, Knn Regressor, Huber Regressor was trained. On all the models trained and validated,Random Forest and Decision Tree had least RMSE. However, due to storage constraint and running time constraint Decision Tree was chosen as it is lighter and faster comparitively.The dataset was tested with test dataset which gave consistent metrics.

**End-Product:**
![app_screenshot](https://github.com/KiruthikaParanthaman/Singapore_Resale_Flat_prices_predictor/assets/141828622/e00dd29f-3bb4-4eaf-8570-4e16f2aeaa90)

Dataset : https://beta.data.gov.sg/collections/189/view

