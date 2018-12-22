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



## Data Analysis 
 #### 1. How likely is the death of a Female person call for a fundraising as compared to a Male person?
 
 ![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/gender.png)
 
 The graph above shows the percentage likelihood of a male and female death calling for a fundraising.We can see that there is no much difference between a female or a male death calling for fundraising. So gender on its own cannot be a deciding factor

 #### 2. How likely is the death of a Married person call for a fundraising as compared to a Single person?

  ![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/Married.png)
  
The graph above shows that it there is no much difference between a married person or a single person's death calling for  fundraising. So Marital status on its own cannot be a deciding factor whether a fundraising will be done

 #### 3. How likely is a Colored obituary predict a fundraising as compared to a black and white one?
 
  ![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/Color.png)
  
  Color of an obituary is also not a good indicator of whether a fundraising will be called or not.
  
 
 #### 4. How does the time between announcement and the burial date affect probability for fundrasing?
 
   ![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/Days.png)
   
  
   The distribution graph above proves that it announcements that are made very close to to burial date are less likely to    likely to lead to a fundrasing as compared to those made far away from the burial date, some are even made as far as 35 from the burial date. 
  
   #### 5.Is size of an orbituary an indicator of a fundraising?
   
   ![alt text](https://raw.githubusercontent.com/nlubalo/Death-Market-Kenya/master/imgs/size.png)
   
  From above distribution, it is safe to say that size of an orbituary is not a very good indicator of whether a fundraising will be done or not. Although from the very far right of the distribution we have a few large orbituaries that are likely to call for fundraising, it is still not very significant.
  
  
   

 
  
