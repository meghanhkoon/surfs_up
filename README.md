# Surf's Up with Advanced Data Storage and Retrieval


## Overview 
***Background***
While trying to start up a Surf and Shake shop in Oahu, investor W. Avy would like to know more about the weather on this island - and if a Surf and Shake shop could be successful. Since W. Avy has previously invested in a similar business that failed due to weather, he wants us to analyze the weather conditions from the island of O'ahu, HI before he invests in our startup company. 

***Purpose***
After the initial analysis, investor W. Avy wants more information about temperature trends. He specifically wants temperature data for the months of June and December in O'ahu to determine if the Surf and Shake shop business will be sustainable/ successful year-round. 

This analysis will use Python, Pandas, and SQLAlchemy to:
- Determine the Summary Statitistics for June
- Determine the Summary Statitistics for December 
- Report our findings with statistical analysis 


## Resources 
- Data Source: Original data ([hawaii.sqlite](https://github.com/meghanhkoon/surfs_up/blob/main/hawaii.sqlite))
- Software: Python, Pandas, SQLAlchemy, SQLite database, Matplotlib, and Jupyter Notebook


## Results

Using Python, Pandas and SQLAlchemy, we first wrote a [query](https://github.com/meghanhkoon/surfs_up/blob/main/SurfsUp_Challenge.ipynb) to filter the date column from the Measurement table to retrieve all the temperatures for the month of June. We then converted the data to a list to create a DataFrame to use the .describe() function to find the summary statistics for the month of June. Lastly, we created a graph using Matplotlib.

To see what the weather is like at the end of the year, we use the same process to find the temperature statistics for the month of December. 

***Summary Statistics for June and December***

![JuneTemps](Files/JuneTemps.png)  ![DecTemps](Files/DecTemps.png)

From our summary statistics for temperatures in June and December on O'ahu, HI, we can conclude: 

1. The average temperature throughout June and December is low 70 degrees (~72.5 degrees). However, in June, we see that the average temperature is 4 degrees higher around 75 degrees vs. December averaging 71 degrees. 
2. June's minimum temperature is 64 degrees and maximum temperature is 85 degrees. December's minimum temperature is colder at 56 degrees but max temperature is similar to June's (83 degrees).  


***Temperature and Frequency Histogram Plots*** 

![JuneTemps_Hist](Files/JuneTemps_Hist.png) ![DecTemps_Hist](Files/DecTemps_Hist.png)

From the Temperature and Frequency Histogram Plots, we found: 

3. The frequency of temperatures recorded in June seem to have a normal bell curve distribution. However, December's temperature distribution does not seem normal. There is a jump in frequency at around 71 degrees, which is also the average of December temps from the statistics summary table. This could be due to there being more data from June (1700) than in December (1517). 



## Summary
In summary, investor W. Avy inquired if O'ahu's temperatures would help make the Surf and Shake Shop business sustainable/ successful year-round. We gathered data from both June and December to see what O'ahu's weather is like during the summer and winter months. From our findings, we see that both June and December have similar average, minimum, and maximum temperature patterns. While December averages 4 degrees colder than June, we know that the median temperatures of each month are very close to their means. 

While the investor only asked for temperature analysis, we know that rainfall (precipitation) will also help our overall weather analysis. To gather more weather data for June and December, two more queries were written to find the precipitation statistics for the months of June and December. From our new queries, we found the statistics summary and plotted the data below: 

![JunePrcp](Files/JunePrcp.png)  ![DecPrcp](Files/DecPrcp.png)
![JunePrcp_Plot](Files/JunePrcp_Plot.png)  ![DecPrcp_Plot](Files/DecPrcp_Plot.png)

From the precipitation table and graphs above, we see that December had an average of .22 inches of rainfall vs. June having .14 inches.  Looking at the precipitation and temperature statistics and analysis, we see that there is no drastic change in weather throughout the year. We can now confidently recommend and prove using our data analysis that the Surf and Shake Shop on O'ahu would be successful year-round. 
