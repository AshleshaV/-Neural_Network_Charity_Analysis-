# -Neural_Network_Charity_Analysis-

## Overview: 
The purpose of this analysis was to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify which organizations should be considered for funding from AlphabetSoupCharity donations. This project compromised of the following methods:

Preprocessing the data for the neural network
Compile, Train and Evaluate the Model
Optimizing the model

## Results: Using bulleted lists and images to support your answers, address the following questions.

#### Data Preprocessing
What variable(s) are considered the target(s) for your model?
The target of IS_SUCCESSFUL is currently the only target for the model.

What variable(s) are considered to be the features for your model?
    -  APPLICATION_TYPE
    -  AFFILIATION
    -  CLASSIFICATION
    -  USE_CASE
    -  ORGANIZATION
    -  ASK_AMT
    -  STATUS
    -  INCOME_AMT
    -  SPECIAL_CONSIDERATIONS

What variable(s) are neither targets nor features, and should be removed from the input data?
  -  EIN and NAME variables.


#### Compiling, Training, and Evaluating the Model
-  How many neurons, layers, and activation functions did you select for your neural network model, and why?

For the initial attempt at model, two layers, with 80 and 30 neurons respectively (both "relu" type) were used.  The activation feature of "sigmoid" was used. 

-  Were you able to achieve the target model performance?

The model performance was set at 75%.  Unfortunately, the current model only achieved an accuracy rating of 74.09% on epochs 96 and 99.  An overall accuracy average of 72.98% was achieved.

-  What steps did you take to try and increase model performance?

In order to improve efficiency, multiple model attempts were performed.  The results of each attempt are listed below:

  -  Attempt 1:
![attempt1](https://user-images.githubusercontent.com/108908214/205534095-f6074793-25cb-49d7-8b2c-b006e409e89e.png)


 -  Attempt 2:
 -  ![attempt2](https://user-images.githubusercontent.com/108908214/205534140-e03ce119-3871-4700-9083-4d432008ed0c.png)


-  Attempt 3:
-  ![attempt3](https://user-images.githubusercontent.com/108908214/205534159-e3011608-4710-45cc-9608-e4b8f5253e38.png)
-  ![attempt3-2](https://user-images.githubusercontent.com/108908214/205534182-03b023aa-e731-43c6-9b45-a4543e573a3c.png)




## Summary:

As shown above, the initial setup for the model did not perform at the required level, coming in at 72.98%.  Through iterative design, the model was adjusted and obtained an increased rating of 73.04% on the second optimization attempt.  All other models had lower final accuracies than the initial model.  For this, it can be seen that changing the number of hidden layers and neurons had a negligible effect on increasing model accuracy.  Further adjustment may lead to an invalid model or one that overfits the dataset.

I would recommend a Random Forest classifier for an alternate model design.  This is due to Random Forest ability of performing binary classification, the ability to handle large datasets, and the reduction in code which can achieve comparable accuracy predictions.
