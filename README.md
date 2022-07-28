# sports-data-analysis
<b>Scraping with Random Sampling:</b>
We randomly sampled hotels from three different cities: Bangkok, Singapore, and Kuala Lumpur. Since we did random sampling, we have to violate some of the guidelines given for this assignment. For example, we can not ignore/remove all the hotels with comments/reviews less than 100 comments while doing random sampling. Some of the hotels in our dataset do not have 100+ comments. We left that as it is. But our average no. of comments was much higher than 100 (see table below). 

![city](https://user-images.githubusercontent.com/79563144/181500771-840e2779-1a03-4dee-b68e-a5d95655c368.JPG)

<b>Factors affected the balance of the dataset:</b>
* While doing random sampling, our sample size can not be more than 10% of the population. This has affected our sample size for Singapore.  
* We have to remove some hotels in the sample after scraping due to data inconsistency. 

<b>Data Analysis</b>

<b>What makes a good hotel?</b>
Is it the wifi? Is it the comfort they provide? Or is it the location of the hotel? We are answering this question with some econometric regression analysis. We regressed the rating for 5 different categories - 	Cleanliness, Comfort, Facilities, Staff, value for money, location, and Wifi - against overall ratings. The coefficient/weights of these categories in the regression give us an idea of what matters and what doesn’t.  I am attaching the actual regression results in the appendix for those people who are interested. 
![data2](https://user-images.githubusercontent.com/79563144/181501324-eeb8247d-7464-422a-97d1-02c308e38ca8.JPG)

With the chart above, we can answer the question we asked above - What makes a good hotel?. As you can see in the chart above, Cleanliness has the highest weight followed by Facilities and comfort. Interestingly, wifi doesn’t seem that important for hotel rating.

<b>Do people not care about wifi?</b>
No, people care about wifi but as much as other categories. Ratings in other categories have a stronger association with overall ratings.  This is best illustrated by comparing the cleanliness and wifi ratings with overall ratings. 
![data3](https://user-images.githubusercontent.com/79563144/181501575-37e1b98d-e11a-47fb-8cc5-659b635a2428.JPG)



