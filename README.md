
# Final Presentation 
![P1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P1.jpg)
![P1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P1.PNG)

## Selected topic

We want to see if we could predict the melting of Arctic Sea Ice using the time series predictive model SARIMAX using Python.

![Header](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/Header.jpg)

## Reason topic was selected

We selected this topic because we wanted to predict at what point in time would the sea ice shrink. It is a topic that all the team members felt passionate about and wanted to explore. 

# Team members 
![P4](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P4.PNG)

# Live Presentation 
Scheduled for 7 pm [EST] Friday, February 9th, 2022. 

![P3](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P3.PNG)

# Final Project Website: 

## [Website Climate Change - Sea Ice Analysis](https://seaiceanalysis.appspot.com/)

# GitHub
## [Final Project Code](https://github.com/ALIYA2Group/Mod20_Segment_3)

### [All Segment Details](https://github.com/ALIYA2Group)

# Google Slides
## [Final Presentation Slides](https://docs.google.com/presentation/d/e/2PACX-1vSV1HhjFlP5gsKDUrtnJqH_iSvr25CP9ZKv9FZbFnaLSPuN6MnA0RDPXdZExbLX_hYIrHlh_7Tc9dz5/pub?start=false&loop=false&delayms=3000)

# Project Overview
![R1a](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R1a.PNG)

# [Database Integration](https://docs.google.com/presentation/d/e/2PACX-1vQ0AFT1H9r4fMRmOl4hKVJDNR87-qmHnjaFkaO2_cpQg13ukkOF0McZ7dscFhhqL2cclg_jVvtWTJui/pub?start=false&loop=false&delayms=3000)

## Description of the source of data

We reviewed data from the following resources and identified the most useful features to be used in our analysis: 

1. [National Snow and Ice Data Center (NSIDC)](http://nsidc.org/data/google_earth)
2. [Climate Data Store](https://cds.climate.copernicus.eu/user/119111)
3. [Visualize Arctic and Antarctic Sea Ice](https://livingatlas.arcgis.com/sea-ice/)

## Here is the Question the team hopes to answer with the data

> Based on past features of science exploration and calculation on melting and atmosphere changes, we extract, transform and load the selected trends to show the sea-ice diminishing from 2003-2020 to try and predict at what point in time in the future these factors would impact the melting of the Arctic sea ice.

## Description of the data exploration phase of the project

* Extract

Through data exploration, we determined that we wanted to use Arctic data only as it is melting faster than Antarctic. 


![R1b](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R1b.PNG)
![D3](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/D3.PNG)

## Description of the analysis phase of the project and data processing

* Transform
 
We had to understand the significance of the science behind the data, to understand which features of the data set we needed to use. When we transformed the features of the data set that were applicable, we reviewed the trends.
![R1c](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R1c.PNG)
![R1d](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R1d.PNG)

* Technologies, languages, tools, and algorithms used throughout the project
![R1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R1.PNG)

# [Machine Learning Model](https://docs.google.com/presentation/d/e/2PACX-1vTU8nhBTVIz_KSLN01zzD6-fK-YunX4blsvz-DwjapgQqs_POwJLEJBWkzrEW5h-C8shGaCReSjNGKS/embed?start=false&loop=false&delayms=15000)

Data pre-processing included importing the dataset using SQLAlchemy from AWS, dropping unwanted columns and setting the date as index.  

## Description of feature engineering and the feature selection, including the decision-making process

The selected features were visualized as time series and against the target (extent) to understand the correlation. 

![CORR](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/CORR.jpg)

## Description of how data was split into training and testing sets

Data was split into training and testing sets using a 70-30 ratio and using the scikit library. 

![traintest](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/traintest.PNG)

## Description of how we have trained the model thus far, and any additional training that will take place
![R3](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R3.PNG)


The model was trained using SARIMAX. After splitting the data into training and testing sets:

1- Decomposed Time Series into several components-Trend, Seasonality, and Random noise

![X1](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/X1.JPG)

2- Checked for Data Stationarity using Augmented Dickey-Fuller(ADF) test. If we make the data stationary, then the model can make predictions based on the fact that mean and variance will remain the same in the future. A stationarized series is easier to predict. For data points that were not stationary, data was differenced to make it stationary. 

3- An ACF and PACF bar chart was plotted. ACF is a plot of the coefficients of correlation between a time series and its lag and helps determine the value of p or the AR term while PACF is a plot of the partial correlation coefficients between the series and lags of itself and helps determine the value of q or the MA term. Both p and q are required input parameters for the SARIMAX Model. 

![X2](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/X2.JPG)

3- Ran the SARIMAX model to forecast the extent based on the order obtained using ARIMA  model and using the traing set as the exogenous variables

4- Fitted the model and trained and tested data was put into a dataframe (converted back to scale)

![F9](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/F9.PNG)

## Description of current accuracy score

The Accuracy Score : 0.08529 (root square mean error)

We resulted in a very good accuracy score.

![F10](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/F10.PNG)

![R3a](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R3a.PNG)

## Future Prediction:

We successfully completed prediction model to predict the features of the Artic Sea Ice melt:

1) A univariate time-series model was applied to each of the features to estimate their future value, which are put into a dataframe

![XFORE](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/XFORE.jpg)

2) using the predicted values of the features, we used the model to predict the values of Y (Extent):

![R3b](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/R3b.PNG)
## Explanation of model choice, including limitations and benefits

Given the nature of the data and the question we are trying to answer, we used a Timer-Series prediction model SARIMAX (Seasonal Auto-Regressive Integrated Moving Average with eXogenous factors). It helps to predict future values using auto-regression and moving average along with adding in the seasonality factor. 

[ARIMA Model](https://www.machinelearningplus.com/time-series/arima-model-time-series-forecasting-python/) - using Using ARIMA model, we can forecast a time series using the series past values. We built optimal ARIMA model from scratch and extend it to Seasonal ARIMA (SARIMA) and SARIMAX models. 

[SARIMAX](https://www.statsmodels.org/dev/examples/notebooks/generated/statespace_sarimax_faq.html) is seasonal updated version of the ARIMA model family.

## Explanation of changes in model choice 

There were a number of different models tried and tested, which were the changes that occurred between the Segment 2 and Segment 3 as follows: 

1. Method using vector autoregression (VAR) 
![M1](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/M1.PNG)

2. Method Time-series forecasting using tensor flow, including convolutional and recurrent neural networks (CNN and RNN)
![M1a](https://github.com/ALIYA2Group/Mod20_Segment_3/blob/main/Pictures/M1a.PNG)

# Dashboard and Website

* Load
 
The website is loaded on python-flask backend and runs on Google App Engine. Our written code used beautiful soup to scrape the news contents from the Ice Data Center scheduled everyday and then store the data into our MongoDB for website loading.

![P3](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P3.PNG)

The daily updated sea ice extent images and sea ice news is scraped from National Snow & Ice Data Center.

![P8](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P8.PNG)

The Data analysis we divided our work into six sections.

![P7](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P7.PNG)

The contents are loaded from MongoDB. Here is our live data, you can see how we store the data in the hierarchical database. 

![P10](https://github.com/ALIYA2Group/Mod20_Segment_4/blob/main/Pictures/P10.PNG)

# Project Summary 

We created the foundation for the final project. By defining roles between team members and establishing a communication structure. We wanted to see if we could predict the melting of Artic Sea Ice. We created a repository for the project and invited the other team members. We made great strides in building the different pieces of the project. The analysis come along nicely, and we worked on the machine learning model, and the databases were transitioned into an operational, data-holding tool. All of the individual pieces we've been building came together. We assembled these pieces, putting the final touches on the repository. Working on the README.md to fully describe the project and its purpose. The repository is ready to be added to our portfolio. The team’s final task is to practice the presentation. Each of us will participate in the presentation over Zoom. All loose ends that have been lingering were tied up especially anything related to the machine learning model, dashboard, or even the analysis. It was a short few weeks to perform ETL, MLT and Website, and we were successful. Based on past features of science exploration and calculation on melting and atmosphere changes we extracted, transformed and loaded the selected trends to show the sea-ice diminishing from 2003-2020 to try and predict future size of the arctic sea ice extent for the next 10 - 30 years. 
