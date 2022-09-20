# Neural_Network_Charity_Analysis


## Overview of Project

In this scenario, Alphabet Soup is non-profit foundation and has been donated to a lot of organizations. They would like to know how those donations are doing to the organizations. We decide to use neural network machine learning to analyze the data. 


### Results

* The target for the analysis is to see if the donation is successfully helping the organization. To be exact, the target variable is “IS_SUCCEFUL”. 

* We keep below features for our model: 
       ”AFFILIATION”,“APPLICATION_TYPE”, ”USE_CASE”, ”ORGANIZATION”, 
       ”STATUS”, “INCOME_AMT”, “SPECIAL_CONSIDERATION, “ASK_AMT”, 
       IS_SUCCESSFUL. We took our “SPECIAL_CONSIDERATION” in the optimal 
       version because there are only 27 for Y but the rest of the data 
       have N.

* We took our EIN and NAME out from the features.  They are just IDs for the data and can’t provide the actual impact on if the donation is successful to the organization or not. 

* We have three hidden layers in the optimal version and each layer has 90,40 and 30 neurons respectively. We stick sigmoid for our output activation function is because it is good for binary classification which is our target for the analysis. We change the hidden layer activation function to tanh – it is a slightly complicated activation function.

* I couldn’t achieve the target 75% accuracy. But we did it close enough -around 72%.

* We add one more hidden layer (the third one), more neurons on each hidden layer, more epochs, take out “SPECIAL_CONSIDERATION” as feature and change the output activation function to tanh.

 

### Summary

The optimal version result is very close to the original version. I have tried different steps to improve the model, however, it is still hard to see the improvement of the model. We might need more data or other effective data to train the model.

It is very time-consuming to train the model. In comparison, this data is still smaller and less feature than the real-world complicated (or size with millions counts database). I would suggest using random forest model. We would have save a lot of time and might achieve the same goal.

 
