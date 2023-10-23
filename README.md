# Project-DNN-Telco-Customer-Churn-Prediction

# About Dataset

The data set includes information about:

Customers who left within the last month – the column is called Churn.

Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies.

Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges.

Demographic info about customers – gender, age range, and if they have partners and dependents


Churn - Whether the customer churned or not (Yes, No)

PhoneService - whether the customer has a phone service or not (Yes,No).

MultipleLines - whether the customer has a multiple line or not (Yes, No, No phone service).

InternetService - type of internet service the customer has (DSL, Fiber Optic, No).

OnlineSecurity - whether the customer has a online security or not (Yes, No).

OnlineBackup - whether the customer has a online backup or not (Yes, No).

DeviceProtection - whether the customer has a device protection or not (Yes, No).

TechSupport - whether the customer has a tech support or not (Yes,No).

StreamingTV - whether the customer has a streaming TV (Yes,No).

StreamingMovies - whether the customer has a streaming movies (Yes,No)

Tenure - how long customer has stayed in company.

Contract - type of contract customer has (Month-to-Month, One Year, Two Year).

PaperlessBilling - whether the customer has a paperless billing (Yes,No).

PaymentMethod - payment method used by customer (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)).

MonthlyCharges - amount charged to the customer monthly.

TotalCharges - the total amount charged to the customer.

CustomerID - Unique value for each customer.

gender - type of gender customer has (Male,Female).

SeniorCitizen - whether the customer is a senior citizen (Yes,No).

Partner - whether the customer has a partner or not (Yes, No).

Dependents - whether the customer has a dependents or not (Yes,No)

# EDA
Follow the EDA section within the jupyter notebook to understand visually how the data is distributed

# Data Preprocessing

# Label Encoding
Label encoding and One Hot encoding is done as per the requirement and is clearly demonstrated in the jupyter notebook

# Feature Scaling
Feature scaling is done using MinMax Scaler

# Splitting the independent and dependent data into train and test datasets

# importing necessary packages to build a DNN model
import tensorflow as tf
from tensorflow import keras
from keras.models import Sequential
from keras.layers import Dense, Dropout, BatchNormalization

# Model Building Approach 1 with imbalanced data
A DNN Sequential Model is built yielding train and test accuracy of 82.90% and 78.65% respectively at 100 epochs

# Model Building Approach 2 with balanced data
A DNN Sequential Model is built yielding train and test accuracy of 81.55% and 80.77% respectively at 100 epochs

# Conclusion: 
It is observed that the DNN model is performing better with the balanced data with train accuracy of 81.55% and test accuracy of 80.77% compared to the imbalanced data with train accuracy of 82.90% and test accuracy of 78.65%. Hence the DNN model with balanced data is showing promising results and can be used in production.




