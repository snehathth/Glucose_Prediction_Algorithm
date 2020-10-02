# Glucose_Prediction_Algorithm
Blood Glucose Level Prediction for Diabetics, based on Glucose Level Logs from CGM, using Personalized Time Series Models

## Overview - Defining Goal
To develop a prediction algorithm that can help the patients to control blood sugar level and prevent hypoglycemia

## Problem Statement
The goal of this study is to understand the data from the CGM and develop a personalized prediction model to predict the patient’s BG level accurately and at regular intervals.

## Understanding Data  
Data of patients who participated in “A Randomized Trial Comparing Continuous Glucose Monitoring With and Without Routine Blood Glucose Monitoring in Adults with Type 1 Diabetes

Blood Glucose Levels were recorded through Dexcom devices. A patient can have up to 288 readings per day as each recording is taken automatically, every 5 minutes 
The data contains the relative day, time and glucose level of each user over a period of ~6 months

## Researching Literature
A lot of papers are present already on the subject matter and it is important to invest some time to understand the methodologies used and the caveats behind each. 

A lot of methodologies including KNN, SVM, DT, RF, RNN were tested. Only very few articles were on time-series. Linear regression with implied regularization is another model that was widely explored. 

The most important metrics conveyed in the evaluation of the models were: 
* RMSE 
* R-Squared 
* Clarke Error Grid 

## Current Results
The experiment results demonstrate that the personalized time series model can give:
* Strong predictions for 10 mins prediction window. MeanAbsoluteDeviation - 2.5 mg/dl
* Do not handle the crests and troughs of the wavy glucose pattern present
* Further research and incorporation of features to understand the impact of carbs, insulin, workout and stress may lead to a robust solution. 
