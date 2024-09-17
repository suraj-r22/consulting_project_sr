# consulting_project_sr
This code contains the cleaning and EDA I conducted for a consulting project I did at UCLA. Our aim was to see if we could find notable differences between stem students and non-stem student experiences, based on class review data from Bruinwalk.com. Essentially, we wanted to see if we could predict whether a class is stem or non-stem based on course ratings and student reviews. Initially, we were also interested in using the text in the reviews for sentiment analysis, so after cleaning the dataset I split it into two distinct datasets for different purposes - one for classification tasks and another for sentiment analysis. Both datasets are present on this repository. 

The first file (final eda) contains the initial cleaning and EDA where I explored the datasets, merged them, made sure the data types were correct, did some text clean-up, and created a function that either classified the observation as "stem" or "non-stem" based on the department name. This allowed me to create the column "Dept.Type" for classification tasks. 

Further cleaning was done in both files present in the repository, which included clearing rows that had missing values for all of the columns and ensuring that one observation did not have more weight than another (some observations had multiple grade distribution data points, so their ratings were duplicated in the datasets - for those data points, I took the average of the grade distributions to have one row present for that class). I used R's tidyverse library for these tasks. 

The second file also contains some classification models I fit to the data, including logistic regression. 

Due to the data being webscraped, it was quite unstructured, so it involved a lot of cleaning. 
