# Neural_Network_Charity_Analysis


## Overview of Project
This analysis seeks to create a neural network to predict which organizations are going to use donations from Alphabet Soup, a charity organization, in an impactful way.



## Results

* Target of the analysis is to see if the donation is successfully helping the organization. 

* Features of the model are:
       ”AFFILIATION”,“APPLICATION_TYPE”, ”USE_CASE”, ”ORGANIZATION”, 
       ”STATUS”, “INCOME_AMT”, “SPECIAL_CONSIDERATION, “ASK_AMT”, 
       IS_SUCCESSFUL. We took our “SPECIAL_CONSIDERATION” in the optimal 
       version because there are only 27 for Y but the rest of the data 
       have N.

* EIN and NAME are taken out of the features.  They are just IDs for the data and can’t provide the actual impact on if the donation is successful to the organization or not. 

* We have three hidden layers in the optimal version and each layer has 90,40 and 30 neurons respectively. We stick sigmoid for our output activation function is because it is good for binary classification which is our target for the analysis. We change the hidden layer activation function to tanh – it is a slightly complicated activation function.

* We add one more hidden layer (the third one), more neurons on each hidden layer, more epochs, take out “SPECIAL_CONSIDERATION” as feature and change the output activation function to tanh.

*  I was unable to achieve the target model performance of 75%, but was close at 72%



## Summary

* The optimal version result is very close to the original version. This model is a fair model for predicting which organizations are low risk to donate to.

* This model could be improved by looking into the most beneficial number of hidden layers or by looking at the dataset and removing any extreme outliers.

* However, it is time-consuming to train the model. In comparison, this data is still smaller and has less features than the real-world complicated data(or size with millions counts database). Random forest model will help us save time and achieve the same goal.
 
