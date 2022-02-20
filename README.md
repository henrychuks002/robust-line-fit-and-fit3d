### Project Analysis
.
### Robust line fit and 3D fit
Regression models predict a numerical value (dependent variable, y) given a set of input variables (also known as independent variables, x). Linear regression is the gold standard for the regression family, it finds the best line (or hyperplane) that best describes the linear relationship between X and the target variable (y).<br />
.<br />
However,in real-world cases, like the example above, the data may contain outliers, and the model fitting can be biased. Robust regression aims at overcoming this (ovecoming the biased fitting). Linear regression models assume that each independent variable follows a Gaussian distribution. A factor that can affect the distribution of the variables when using a linear regression model is the presence of outliers (samples that are far away the expected distribution, and can cause problems to a linear regression model, from Fig 1.1 and 1.2 below, the "red" data points represents the outliers available in the data). This results in models that are not performing well and that are highly biased and influenced by the underlying outliers. To overcome this, robust regression algorithms is used as the Random Sample Consensus Regression(RANSAC) model. The ransac model is a well known robust regression model and it tries to separate data into outliers and inliers, and it then fits the model only on the inliers. <br />
. <br />
The artificial dataset used in the robust line fit program consist of a dependent variable (y) and an independent variable (x) with 400 observations from negative 200 to 200 which also includes outliers.<br />
.<br />
![robust_line_result](https://user-images.githubusercontent.com/65792408/154846140-cb7602e2-40ec-4d4c-a8d4-afb9615a2223.png) <br />
Fig 1.1 <br />
.<br />

![robust_3d](https://user-images.githubusercontent.com/65792408/154846764-a6cfa30b-0b87-422a-bbf0-98228c855cb7.png) <br />
Fig 1.2 - Representation of the model fit in 3D.<br />
.<br />
From the Fig 1.1 and 1.2 above, we can observe that the robust regression model performs well in fitting the inliers (blue datapoints) and ignoring the outliers (red datapoints). The presence of outliers in a dataset can introduce bias and lead to underperforming linear regression models. To deal with these outliers, the robust regression algorithm can be used. We can also observe from the image above that robust model can perform well enough when outliers are present, whereas regular linear regression model may highly be affected and biased by these outliers. 
