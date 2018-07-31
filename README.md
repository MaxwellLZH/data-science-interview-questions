# Common Data science interview questions and answers


### What is regularization? The differences between Lasso vs Ridge?
- Regulization is a process of adding a tuning parameter to a model to induce smoothness of the weights (prevent the coefficients to fit so perfectly) in order to prevent overfitting.
- Lasso formula:  
![LASSO formula](http://www.chioka.in/wp-content/uploads/2013/12/least_squares_l11.png) 
![](picture/lasso_regulization.png)  
<hr>  

Ridge formula:  

![Ridge formula](http://www.chioka.in/wp-content/uploads/2013/12/least_squares_l2.png)   
Lasso vs. Ridge comparison:  

![Comparison](http://www.chioka.in/wp-content/uploads/2013/12/L1-vs-L2-properties-regularization.png)   

![Ridge picture](picture/ridge_regulization.png)       

<hr>
Check out this wonderful post: [Differences between L1 and L2 as Loss Function and Regularization](http://www.chioka.in/differences-between-l1-and-l2-as-loss-function-and-regularization/)  


### Derive the ordinary least square regression formula
[Derivation](http://cs229.stanford.edu/notes/cs229-notes1.pdf)


### How to deal with overfitting?
1. Train with more data  
2. Cross validation  
3. Do feature selection  
4. Use early stopping if possible  
5. Regulization  
6. Ensembling  
Reference: [overfitting in machine learning algorithms](https://elitedatascience.com/overfitting-in-machine-learning#how-to-prevent)


### If I double every sample observation in a linear regression model, how will the coefficients, r-squared value and t-value change?

Coefficients will be the same (obviously).

Let's consider what is r-squared value?
[Here](https://onlinecourses.science.psu.edu/stat501/node/255/)'s a detaild introduction to r-squared.
> "r2 ×100 percent of the variation in y is 'explained by' the variation in predictor x."
Scaling the sample doesn't affect Xi's ability to 'explain' Y, so the r-squared should remain the same.

t-value will be sqrt(2) times bigger which is pretty obvious from the fomula of t-value: 

![t-value](pictures/t_test.png)  


