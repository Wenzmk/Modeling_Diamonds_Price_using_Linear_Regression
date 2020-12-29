# Modeling_Diamonds_Price_using_Linear_Regression
This is one of Bangkit Traning Program Project.
Using Linear Regression to predict diamonds price.

### Required Libraries
analysis was performed using Python 3 at Google Colab Notebook. Please make sure that the followings libraries is already installed:
1. pandas
2. numpy
3. matplotlib
4. sklearn
5. tensorflow

### About Data
The data are the secondary data took from Kaggle: [Diamonds](https://www.kaggle.com/shivam2503/diamonds).

Context

This classic dataset contains the prices and other attributes of almost 54,000 diamonds. It's a great dataset for beginners learning to work with data analysis and visualization.

Content
1. price price in US dollars (\$326--\$18,823)
2. carat weight of the diamond (0.2--5.01)
3. cut quality of the cut (Fair, Good, Very Good, Premium, Ideal)
4. color diamond colour, from J (worst) to D (best)
5. clarity a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
6. x length in mm (0--10.74)
7. y width in mm (0--58.9)
8. z depth in mm (0--31.8)
9. depth total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
10. table width of top of diamond relative to widest point (43--95)

### Description
Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. One variable is considered to be an explanatory variable, and the other is considered to be a dependent variable. For example, a modeler might want to relate the weights of individuals to their heights using a linear regression model. For the detail about Linear Regression click this following Link [Linear_regression](http://www.stat.yale.edu/Courses/1997-98/101/linreg.htm).

### Result
There are two features that have a same high correlate to diamond price, they are carat and volume(xyz). We make 3 models, they are:
1. Carat Vs Price (loss: 199733.0156- root_mean_squared_error: 446.9641)
2. Volume Vs Price (loss: 27.8366 - root_mean_squared_error: 5.2762)
3. Cross feature (Carat and Volume) vs Price (loss: 35.8933 - root_mean_squared_error: 5.9963))
The best simple linear regression model is the model of Volume Vs Price, because have the smallest Loss and RMSE. The Simple Linear Regression Model of Volume Vs Price is
Price=(-8.5994)+0.2576(Volume)
