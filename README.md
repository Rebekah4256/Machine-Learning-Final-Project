This is the final project for my machine learning class about the quality of wine.

The data I am using is https://archive.ics.uci.edu/dataset/186/wine+quality, and the original creators of this data are Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Wine Quality [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.

My goal with this data is to create a machine learning model to predict the quality of wine.

First, I needed to find out more about my data, so to start, I made a bar graph to learn how balanced the data is. From the bar graph, I found that the data is quite skewed, as it shows that there are way more wines of 6 and 5 quality than any others.

Next, I wanted to look at a correlation heat map to see if there were any strong correlations between any of the columns. What I'm seeing from the heat map is that there are quite a few strong to medium correlations between many of the variables, for example, total sulfur dioxide and residual sugar is at .5.

After that, I wanted to see the relationship between the quality of the wine and the alcohol percentage. To show this, I chose to use a box plot, and it does seem that there is a pattern showing that the alcohol percentage may have a pretty big impact.

Finally, for the EDA, I wanted to see what the relationship is between sulphates, volatile acidity, and alcohol percentage. I chose to show this as a paired scatter plot with the colors of the graph being the wine's quality, showing how differing data points are related and how the quality of the wine differs between each graphed variable.

Now it was time to choose, and make the machine learning models for the first ML model. I chose to do a KNN learning model. I think that this is a good choice for this data because it takes into account multiple variables. And for the second, I chose to use a Random Forest classifier, as I think that this is most likely the best choice for predicting the quality of a wine.

To make the KNN model, I first needed to get my X without my target (quality), and then I put my target into y. Next, I needed to scale the data. After that, I then fit the data to the model, and when run with the neighbors being 14, I got the model to have an accuracy score of 56%, so it's not the best model, but it's slightly better than a guess.

Then, with making the random forest classifier, I again got my X and y fit to the model, but with this type of ML model, I did not need to scale the data, so I skipped that. When I run this model set with estimators at 20 and with a max depth of 28 (I found these numbers with a little trial and error), I get an accuracy of 67%. So overall this was a much better ML model for this data.
