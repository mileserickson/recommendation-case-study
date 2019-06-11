# The Task:
We are to build a movie recommendation system for a potential client. This system should serve current users as well as new users.
<br>
## The Data

We have been provided movies.dat, movies_metadata.csv, ratings.json, and users.da to use to build a model.

## The Plan
Use Spark and Pandas to put the information into dataframes, then use ALS to see recommendations for users with previous ratings as a baseline. Then move forward to deal with new users. 

## The Preperation
Deal with incorrectly formated id's, StandardScaling, OneHotEncoding, 40000+ null values (We ended up splitting our data into 2 sets, one with null filled rows removed: X2, the other with null filled columns removed: X3)

## The Modeling
We use both a Neural Network and XGBoost on each of our datasets to deal with the cold-start problem for new users.

## The Results
For X2: Our Neural Network had an accuracy of 35%, while XGBoost had an accuracy of 36%.
For X3 we also had 35% accuracy with a Neural Network.



