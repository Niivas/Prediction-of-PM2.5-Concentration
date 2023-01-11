# Prediction-of-PM2.5-Concentration-
Prediction of PM2.5 concentrations based on meteorological parameters using various regression algorithms.
1. We have taken meteorological and pollutant data from two locations; Safdarjung, New Delhi, and Vishakhapatnam. Meteorological parameters of both New Delhi and Vishakhapatnam are collected from a website called tutempo.net. Data from the year 2016 to 2019 is collected.
2. Metrological data parameters collected are:
```
  -T   - Average Annual Temperature (°C)
  -TM  - Annual Average Maximum Temperature (°C)
  -Tm  - Annual Average Minimum Temperature (°C)
  -SLP - Atmospheric pressure at sea level (Pa)
  -H   - Average relative Humidity (%)
  -V   - Annual average wind speed (Km/h)
  -VV  - Average visibility measured in (KM)
  -VM  - Maximum sustained wind speed (Km/h)
```
3. Pollutant concentrations such as SO2, NO2, and CO for both New Delhi and Vishakhapatnam for the respective year are taken from kaggle website.
4. We made different datasets for model training with only meteorological parameters of New Delhi’s meteorological data, two datasets with both meteorological data and pollutant concentrations of New Delhi and Vishakhapatnam.
5. Datasets for each season such as summer, winter, and monsoon for both New Delhi and Vishakhapatnam to study the influence of meteorological parameters on the concentration of PM2.5 pollutant. 
6. The data that is collected is cleaned and pre-processed. All the records are which contain null values are dropped. Then feature engineering is done to extract important features from the dataset. In this, we can remove independent features if more than one feature has the same correlation with the dependent feature.
7. Heat map and pair plot from the seaborn library is used to find the correlation and trend between dependent feature and independent features. Data is split into 70% for training and 30% for testing. In this study, we have used five regression models to train the data and predict PM2.5 concentration.
8. Those are multi linear, Ridge, Random forest, Xgboost, and ANN regressor.
