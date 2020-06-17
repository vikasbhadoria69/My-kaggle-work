Used cars price prediction using Machine Learning.

I have used the kaggle dataset here. 
Dataset link: https://www.kaggle.com/avikasliwal/used-cars-price-prediction

Here’s the highlights of what I did in this project :

1. Created new features which could be helpful e.g. I created the feature Manufacturer from Name.

2. Tried different approaches to handle the same column. The Year column when used directly produced bad results so I instead used the age of each car derived from it which was much more useful. New_Price was first filled with average values based on Manufacturer but it was not useful, so I dropped the column.

3. Columns that seem irrelevant should be dropped. I dropped Index, Location, Name and New_Price.

4. Creating dummies requires handling of missing columns in test data.

5. Played around with the parameters of the ML model as it can be useful. RandomForest gave me the better results. So I applied RandomizedSearchCV for finding the best parameters. The tuned model gave me better results.

Anyone forking this repo can try to use different EDA techniques and used other models such as XGboost. 
Let me know if you find a better approach which I am sure there will be. :)