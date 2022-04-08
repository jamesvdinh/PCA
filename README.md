# Principal Component Analysis (example using weather data)
A project regarding the concept of Principal Component Analysis (PCA), a method for reducing the dimension of massive data sets onto a projected vector  

Even if you aren't a mathmetician or data scientist, you've probably encountered some sort of visualized data set, one that was much too complicated to make much sense of. Yet, the idea of **Principal Component Analysis** is to condense those data points into a simple array of understandable info. An example can be used with **vector projections** which projects vectors of a certain dimension onto a 2D-space "direction" line vector. This line would include a projection, in the sense of assigning a "score" or "grade," to the data point, thus helping to better visualize the position of the data point in relation to the rest of the set. Vector Projection does not represent the value of the data point as much as it offers a relationship with other data points in the set.


# Senator Voting Data [Example]
Placing this into perspective, we can better understand how much a certain selection of points in a set are skewed towards one quality or the other, such as in a relation of sentator voting patterns. The image below represents a matrix of all the votes of US Senators in from the 2004-2006 term of 645 bills. Each row represents the votes of a single Senator, and each column represents the vote distribution of a single bill. The __Dark__ areas represent 'Nay' on a bill while the __Blank__ areas reprsent 'Yay' with __Gray__ representing an abstain. From the chart below, the data isn't very useful in determining the political biases of senators on a specific scale. Thus, we can use PCA projection to simplfy these data points into a more concise model.

![Senator Data](SenatorData.png)

By using an equation which takes the summation of all the votes of a specific senator, and calculating the **average**, we can assign a "score" to each, thus placing each senator in relation to one another and helping to determing political patterns. If each 'Nay' vote is given a value of -1 and each 'Yay' vote is given a value of 1 with each abstain given a value of 0, the average of these votes on each bill will represent the score of the senator. Comparing this example to vector projection, our "direction vector" is the score of the average bill in the set with a zero-mean score, meaning the vector of sample averages of the different data points. By plotting these scores on a single 2D visualized chart, were presented with a projection of the Senator voting data, which can determine the bias of each senator attributed with their political affiliation.

![Senator Projections](SenatorProjection.png)


# Project
Using Python and the MatPlotLib library, I created a program that took vectors, calculated their projections, and plotted those projections on a predetermined line.

Main Program: WeatherData.ipynb
