# kaggle-spaceship-titanic
So this was my first attempt at using machine learning without using any form of tutorial. 
The problem I was trying to answer was a different version of the Titanic, it proposed that if the Titanic was in space and encountered some anomaly and was destroyed.
The question was which passengers would survive?

Link to the problem: https://www.kaggle.com/competitions/spaceship-titanic/overview

# The model
The model I made ended with about ~73% accuracy on which passengers would make it out alive. I used a RandomForestRegression model from the Sklearn library.

In this question there were a lot of NaN values that I had to deal with, my first attempt I tried to drop all columns that contained a NaN value but as there were over 1000 columns
I realized that I needed to find a different way. On my second attempt (which is the file I uploaded here) I used sklearn's imputer set to most_frequent.
In short what it did was fill any NaN values with whatever the most frequent number of that column was. 

