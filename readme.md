# Cryptocurrency Pump-and-Dump Detecting

This repository contains created dataset and overall analysis for my master thesis:
Cryptocurrency Pump-and-Dump Schemes, Detecting, Modelling and Forecasting, 2023

## The dataset

The dataset contains a list of pump and dumps arranged by groups on Telegram, the final version that was used in empirical analysis can be found in the folder "feature", the file is called "features_labelled_and_available_final.csv". See the paper (will add soon) for a more detailed description of the dataset generation process. The pump events are listed inside the folder мanually_collected_data, the file is called "P&Ds.csv".

## Empirical research

All steps to collect the data can be found in JupiterNotebook "P&Ds_create_data.ipynb". All analysis can be found in "P&Ds_analyze_data.ipynb". 

## Models

In this paper we used the following models:
* SVM
* Random forest
* C-LSTM

## Short description of folders:
* data - Folder that consists all transactions for up to 2 days preceding and succeeding each pump
* features - Folder consists 3 different datasets: without laballed target variable and all 76 pumps "features_nolabaled_15S.csv", without laballed target variable and 43 pumps "features_nolabaled_and_available_15S.csv", and  with laballed target variable and 43 pumps  "features_labelled_and_available_final.csv"
* models - Folder consists C-LSTM model settings
