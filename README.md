# Gym Visitors

# Project motivation and description
In this fictional scenario (with real data), the stake holder is a gym owner at a university campus who is looking to use these data to improve marketing/promotion strategies, as well as to save money by optimising staffing (i.e. schedule in less staff when the gym is quiet). 

# Questions
1. What are the most/least popular times to visit the gym throughout the year?
2. What are the most/least popular times to visit the gym throughout each day?
3. Given the day of the week, the week number, the time,  and the temperature, can we predict how many people will be visiting the gym?

# Outcomes
- There are clearly certain periods in the year that are busier than others. The gym owner can use this information to try to improve customer retention through marketing/promotion strategies. For example, it seems that gym visits decrease from around calendar week 12 onwards. This might be a good time to offer promotions that can help retain customers (e.g. certain goodies when extending contract). We also see that gym visits increase from around week 34 (likely due to the semester start). This might also be a good time to offer certain extras for people signing up for the gym, in order to potentially attract more new members (e.g. first four months free).
- The data shows that certain time periods (e.g. between 3 and 10 pm on most weekdays) are more popular than others (e.g. weekday mornings). This can help the gym owner to schedule staffing more efficiently. There may also be an opportunity here to try to distribute visitors more over the day (very busy gyms are likely less comfortable for visitors). The gym owner could consider offering discounted gym membership that only allows entrance before e.g. 3 pm.
- The KNN regressor (R-squared = .76) and the Random Forest regressor (R-squared = 0.79) both do alright at predicting the number of visitors at the gym considering the week number, the time of the day, the day, and the temperature. The performances of these models may be improved through better data quality (see below) and experimenting with hyperparameter tuning and using different types of models. Already, however, the gym owner can use this to better predict required staffing at a given time of day. 

# Future work
- I would like to ask the gym owner for more data from different years, which will help make these outcomes more reliable.
- I would like to ask the gyn owner whether he has access data for each individual visitor (e.g. through scanning a tag or QR code when entering the gym). This will allow for much more reliable calculations on the number of people that are present in the gym at any given time (with the current data set I have had to calculate this using the mean of the ten-minute visitor numbers), which means that people may have been counted more than once. 
- I would like to use the KNN regressor or the Random Forest regressor (depending on which one proves more accurate with more data) to develop a tool on the gym's website/app which allows customers to check crowdedness at the gym as well as recommend times that will likely be quiet. This may help encourage customers to come in at times that are less busy, thereby improving distribution of visitors across the day. 

# References
Data taken from: https://www.kaggle.com/datasets/nsrose7224/crowdedness-at-the-campus-gym
