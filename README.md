# Movie-Correlation
IN THIS PROJECT WE LOOK AT WHAT VARIABLES EFFECT THE GROSS REVENUE FROM MOVIES.

By my predictions it could be movie's budget and company's name.
Let's check it! Please open the ipynb file and see for yourself

At first i am exploring the data and I noticed that there are some missing data. There are many ways to handle missing values but for the sake of time, I
decided to drop all rows that have missing data. Running the following:
  df = df.dropna()
  
I'm gonna see if movie's gross affects to movie budget. After sorting table by table, i create a scatter plot. The coordinates of each point are defined by 'Gross for film' and 'budget earnings' and filled circles are used to represent each point. This kind of plot is useful to see complex correlations between two variables. 
Then i am overlaying scatter points with a linear regression model and looking for relationship trends between two variables using: 
regplot()
We see that gross and budget positively correlated.
Then i compute pairwise correlation by standard Pearson method(only for numeric features ar first) and to be it more colourful i decided to visualize this data by heatmap.
As i predicted 'budget' has the highest correlation, but it happened that also 'votes' has high correlation.

I wanna chech if company's name has high correlation. 
For that i need to numerize not numeric features.  And after doing the same processes, i see at heatmap that company's name has low correlation, which means my predictions about it was wrong.

