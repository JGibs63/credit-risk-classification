# credit-risk-classification

<h2>Overview</h2>

The purpose of this analysis is to walk through the results from two different prediction methods, and to decide which one is best suited to predict loan risk. I utilized both the linear regression method as well as the logistic regression method.

<h2>Analysis</h2>
From the lending data given, I was able to separate the data into features (characteristics used to create predictions) and labels (the outcomes). From there, we trained and tested the machine with the current dataset in order to create a linear regression model. The linear regression model shows us essentially a trendline that the data should follow according to characteristics given in a loan application. With this model and the original dataset, the results were the following:

Healthy loans: 
- Precision Score: 1.00
- Recall Score: 1.00
- F1-Score: 1.00

High-Risk loans:
- Precision Score: 0.86
- Recall Score: 0.91
- F1-Score: 0.88

Healthy loans had 15,001 occurrences while high-risk loans had just 507 occurrences. The overall accuracy is 99%, and the balanced accuracy  score which gives equal weight to both types of loans is 95.21%.

Moving onto the next method, logistic regression, we wanted to over-sample the original dataset to give the machine a larger dataset to work from. With this model, healthy loans and high-risk loans had 60,035 occurrences each. The results from this method are the following:

Healthy loans: 
- Precision Score: 1.00
- Recall Score: 0.99
- F1-Score: 0.99

High-Risk loans:
- Precision Score: 0.99
- Recall Score: 1.00
- F1-Score: 0.99

The overall accuracy and the balanced accuracy score were both 99%.

Even with the small (<=1%) dip in prediction healthy loans, the logistic regression method was able to predict high-risk loans with a higher accuracy and precision of 99%, and raised the balanced accuracy by 4%. Given these results, it is clear that the logistic regression model should be used in order to have a higher prediction accuracy overall, and specifically for high-risk loans.
