# surfs_up Analysis

## **Overview of analysis**

Our analysis is regarding understanding the weather of the beautiful island Oahu in Hawaii to further analyze how successful would be the investment on surf n shake store in that particular island. The analysis is done on the data provided by the potential investor who is concerned about how the weather might impact the business.

## **Results**

1. In the months of June and December the minimum temperatures are 64 and 56 respectively.

2. The maximum temperatures in the months of June and December are 85 and 83 respectively.

3. From the maximum temperatures, minimum temperatures and other values in the summary of statistics we can deduce that in the months of June and December the average temperatures are between 70 to 75 which is fairly a good weather for Surfing as well as ice creams.

![alt text](https://github.com/LaharikaSCU/surfs_up/blob/main/Histogram_Dec_Temps.png)

![alt text](https://github.com/LaharikaSCU/surfs_up/blob/main/Histogram_Dec_Temps.png)

4. From the data available we can also notice that precipitation is less in June compared to December. In turn, both June and December have less precipitation in comparison with all the months year round, July being the month with highest precipitation of 11.53.

5. Queries for precipitation statistics for the months of June and December:

session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==6).all()

![alt text](https://github.com/LaharikaSCU/surfs_up/blob/main/Precipitation_statistics_June.png)

![alt text](https://github.com/LaharikaSCU/surfs_up/blob/main/Precipitation_Statistics_Dec.png)

session.query(Measurement.date, Measurement.prcp).filter(extract('month',Measurement.date)==12).all()



## **Summary** 

 
Analysis shows, the average temperatures in Oahu islands is between 70 to 75 all year round including the months of June and December. The precipitation is less in months of June and December and high in July compared to the other months year round. The weather conditions seem to be fairly favorable for surfing in OAHU almost all the months year round hence, the Surf N Shake store will sustain long.