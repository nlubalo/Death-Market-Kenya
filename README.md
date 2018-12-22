# Death-Market-Kenya

You have been provided with data on mortality in Kenya. This data can be useful in informing products for life insurance products. There are several analysis that can be conducted to enable make better decisions for creating and marketing of life insurance products.<br>
Can we use this information to tell whether a fundraising will be held for the funeral? 

## Data Cleaning
The dataset has total of total of ***1291*** data points ***39*** features. It has alot of missing fields and data entry errors that need to be sorted before any analysis can be done on it.

The bar graph below shows the percentage of missing data for each feature. We can see some faetues have close to 100% missing data. 

![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/missing_data.png)

The first step I took to removing these NaNs was to drop all features with above 20% missing data. This left me with 19 out off the total 39 features.<br>
I then dropped off all NaNs in the Fundrasing feature. I need it completely flled up since its the feature we need to predict.
<br>
This left only 8% of data missing in the dataset so I dropped off all the NaNs leaving us with ****929**** data points and **19** features.

Other data cleaning carried out are:
-Converting categrical features from texts to integer encoders
-Cleaning the data entry errors like in spellings like ***weekend*** and ***weeekend***, which makes these two appear like different entries.

More on data cleaning can be found in the ***data_cleaning*** notebook file






