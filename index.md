## Coronavirus Cases Affecting the Country of Timeseria

The coronavirus, also known as COVID-19, needs very little introduction as it has been running rampant across the globe for some time now. 66 days have passed since the first confirmed case entered the country of Timeseria and the COVID-19 case count has since been increasing at an impressive rate, reaching just over 30,000 total confirmed cases to date. The upward trend in total cases can be seen in the figure below.

![Total confirmed COVID-19 cases in Timeseria](https://user-images.githubusercontent.com/64803890/81004446-46abd800-8e01-11ea-8049-baeba0c847dd.png)

Citizens of Timeseria have expressed concerns regarding hospital space and equipment, as well as the economic effects of a global pandemic. In order to inform decision making regarding the spread of COVID-19, we have fit different models to the current dataset and estimated a 10-day forecast. Of the models considered, we selected a model that fits the data  well while also giving us good predictions for the future. 

The model we selected is an ARIMA(1,3,1) model that is fit to a logarithmic-like function of data. Though this acronym may seem intimidating and the exact model details are complex, the basic intuition of the model is straightforward. The three in the model accounts for the upward trend of the data. When exploring the dataset, we found there was a trend, a trend of the trend, and even a trend of the trend of the trend. To our more math inclined audience, the modified data roughly resembles a cubic polynomial. The first one indicates that the transformed data relies “linearly” on the previous data point (each data point is “something” added to a previous data point), and the second one implies that the randomness of the previous data point has an effect on the randomness of the current data point. The ones in the ARIMA(1,3,1) model essentially take into account the correlation between data points. 

Based on our model prediction, we estimate the total COVID-19 case count will reach approximately **110,000 within the next 10 days**, which is shown on the figure below. 

![Predicted COVID-19 case count in the next 10 days](https://user-images.githubusercontent.com/64803890/81121823-797acc80-8ee4-11ea-8e56-f6e9bb4a8b7e.png)

According to our 70 percent confidence interval, the total case count could range from approximately 38,000 to 320,000 in the 10-day period; furthermore, the upper limit of our 95 percent confidence interval shows that the total case count could reach numbers on the order of 800,000. Perhaps this model’s biggest flaw is that it does not account for changes of behaviour like social distancing, herd immunity, or that our population is not infinite. So this model cannot be used for long-term predictions, but we believe it is useful for short-term forecasts. Despite the relatively large range of uncertainty, these numbers demonstrate the importance of measures taken to reduce the rate of the spread, such as social distancing and a possible shelter-in-place order. 



_Written by: Tessa Williams, Rex Winn
Date: May 6, 2020_
