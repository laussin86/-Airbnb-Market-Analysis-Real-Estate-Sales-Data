# 🏠Airbnb-Market-Analysis-Real-Estate-Sales-Data
- **Project Summary:**

  The project aims to analyze the impact of Airbnb on the real estate market using sales data. By combining market analysis data with Airbnb listing information, the project seeks to uncover insights into how the revenue of airbnb increase or decrease based various variables like occupancy  in various neighbourhoods.

- **Exploratory Data Analysis (EDA):**

1. Identifying spatial patterns and trends in Airbnb listings.
![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/dadc964a-7b5a-4d5b-9950-882cafbc001a)

3. Exploring the distribution of amenities (e.g., hot tubs, pools) among Airbnb properties.
   ![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/4d541a4f-5421-4674-91d8-3b94f0f34ee8)
   ![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/f10719cb-6161-4daa-83e6-822a36bbb94c)
  We can notice the trend of hot tubs was declining over the motnhs and years while the pools remain constant. that's it is the indication that consumer prefer pools than hot tub.

4. Analyzing the relationship between  Airbnb Revenue and occupancy rate,city and zone.
   ![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/e416762c-66e4-4ac3-8297-1fc6da7dde75)
   ![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/3b01c2a8-6e73-461f-8d22-1348f3b11f20)
   ![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/ac080589-ca8c-436d-b836-640e2f94de56)

- **Model building:**

  I build a model to predicted the occupancy rate based on the other features. the goal of that is to see the occupancy rate we need to have if we want to have a specific revenue for our property of course based on our location, property amenities etc..

we used an XGboost for our model because it is a robust tools and can handle efficiently outliers and missing values. our model gave us a MAE(mean absolute error) of ~0.06.It presents a value that is easy to understand; it shows the average value of model error meaning on average, XGBoost will predict a value that is bigger or smaller than the true value by 0.06 which is good. 

with the visualization of our learning curve for training and test, we can see that our model is not overfiting and predict pretty well: 
![image](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/bb7f956c-709b-4676-9488-e673a00db4d4)
![Screenshot 2024-05-31 151015](https://github.com/laussin86/-Airbnb-Market-Analysis-Real-Estate-Sales-Data/assets/99372300/6a188a9b-4f4e-43f4-b8f8-f913908196ef)

- **Market Insights and Recommendations:**
  
Based on our analysis, we can see that pool is more popular than hot tub and investor need to focus in certain area if they want to maximise their revenue as an Airbnb property owner.

- **Limitations:**
  
1- The datasets might not be representative of the entire real estate market or Airbnb ecosystem, as they only include certain geographic areas or property types so further research for more diverse data will generalize more the result. 

2- The analysis is not capture temporal fluctuations in Airbnb activity and real estate market conditions, as the datasets are limited to specific time periods. Changes over time, such as seasonal variations or market trends, could influence the results.

3- The granularity of location data (e.g., latitude and longitude) may not be sufficient to capture fine-grained spatial patterns and neighborhood-level effects on property prices and Airbnb demand.

- **Future research:**
  
1- Conducting a longitudinal study to track changes in Airbnb activity and real estate market dynamics over time could provide insights into the evolving relationship between the two sectors. Long-term trends and cyclical patterns could be identified, allowing for more robust predictions.
  
2- Augmenting quantitative analysis with qualitative research methods, such as interviews or surveys with property owners and residents, could offer deeper insights into the social and economic impacts of Airbnb on local communities.

3- Exploring advanced machine learning techniques, such as natural language processing (NLP) for analyzing Airbnb listing descriptions or image recognition for property photos, could enhance the predictive power of the analysis. These techniques could uncover hidden patterns and features influencing Airbnb performance.
  
 
