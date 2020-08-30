# Estimating price of Used Cars
This ML project helps estimate the price of a used car, provided by the UsedCars.csv Dataset.

## Various Steps Involved:
1. __Analyze the data__ : Data is first retreived using pandas and the dataframe is prepared. Relevant questions are then asked, upon which relations between the features are derived.  

1. __Visualisation of data__ : Using the relations obvious to the naked eye or derived by compaison, a variety of line, scatter, pie and bar plots are prepared. Using the plots, conclusions are drawn.  

1. __Feature Engineering__ : This step involved the *cleaning* process of the data. Null values were filled and data types were modified. Relations between price and other features were derived. Based on this, unwanted features were dropped. Categorical features were then one-hot encoded.  

1. __Pre-Processing__ : The dataframe was split into X_data and Y_data, where X_data were the features and Y_data was the price. These dataframes were further split into training and testing data sets. The data sets were normalized for uniformity.  

1. __Estimation Models__ :
      
      1. __Linear Regression__ : Linear Regression was implemented on the data sets. Approximate values:
          * Training Loss: ~23.3839 * 10^-4
          * Test Loss: ~23.5090 * 10^-4
          
      1. __Neural Network__ : A neural netwrok with 2 layers and 64 neurons each was created. Approximate values:
          * Training Loss: ~20.3242 * 10^-4
          * Test Loss: ~20.0403 * 10^-4
          
      1. __K-Means Clustering__ : The X_data was clustered with 3 centers:
          * Low price range
          * Med price range
          * High price range  
          
       The elbow plot did not indicate any obvious elbow, so clusters were concluded at 3 for a fair estimate.
          
## Packages Used:
* Numpy
* Pandas
* Matplotlib
* Seaborn
* Scikit Learn
* Keras



