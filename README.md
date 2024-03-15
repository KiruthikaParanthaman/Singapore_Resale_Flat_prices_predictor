# Singapore Resale Flat Prices Predictor
**Problem Statement:**
Singapore Housing and Development Board(HDB) has dataset of resale flat transactions from 1990 to till date. Objective of this project is to to develop a machine learning model and develop a user-friendly web application that predicts the resale prices of flats in Singapore.This predictive model will be based on historical data of resale flat transactions, and it aims to assist both potential buyers and sellers in estimating the resale value of a flat.

**Tools and Technologies Used:** 
Python,Jupyter Notebook,Streamlit

**Model-Building Approach:**
Dataset from Singapore Housing Development Board was downloaded from 1990 to March-mid 2024. Datasets in csv format converted to dataframe and Exploratory Data Analysis was performed before merging all the datasets into single dataframe.Missing columns like 'Remaining Lease' was featured using available data of Transaction date and Lease Start date. Null values,outliers and datatype compatibility checked.After Datatype conversion datsets were merged. Based EDA, new column "Building_age_today" which specifies building age of Flats based on Lease commencement date was calculated.Columns with no useful information like "block" was dropped,followed by Label Encoding,Standardization,Model-building and deploy streamlit app. Complete EDA description could be accessed (here)[https://github.com/KiruthikaParanthaman/Singapore_Resale_Flat_prices_predictor/blob/main/Project%20Singapore%20Resale%20Flat%20Price.ipynb] 
