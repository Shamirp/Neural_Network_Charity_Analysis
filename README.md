# Neural_Network_Charity_Analysis

## Overview of Analysis 

Using machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

### Optimized Model 
![NN](https://user-images.githubusercontent.com/88383836/148804739-4bfaf0c0-bb37-4728-bb85-b665420e9caf.PNG)

### Accuracy and Loss Percentage
![Acc](https://user-images.githubusercontent.com/88383836/148804848-13a13a1b-8c8a-42eb-8849-d7bee2a6d360.PNG)

## Results 

### Data Preprocessing

	What variable(s) are considered the target(s) for your model?

•	Our target in the model are the successful applicants. 

	What variable(s) are considered to be the features for your model?

•	The features being queried are the APPLICATION_TYPE, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, STATUS, and AFFILIATION

	What variable(s) are neither targets nor features, and should be removed from the input data?

•	A few features that were dropped initially were the EIN and NAME these were removed to avoid over classification of our model.

### Compiling, Training, and Evaluating the Model

	How many neurons, layers, and activation functions did you select for your neural network model, and why?

•	The optimization model created used two layers and two different activation types “relu” and “sigmoid”. Using a dense layout, the first layer used 80 neurons and the second layer used 30 neurons. I attempted to use higher and lower number of neurons to test the accuracy of the model and both attempts ended with a higher loss percentage and a lower accuracy percentage. 

	Were you able to achieve the target model performance?

•	The highest accuracy score I obtained with my optimized model was 73%. This did not reach the target goal for the model of 75%. 

	What steps did you take to try and increase model performance?

•	I attempted taking out multiple features in the dataset to attempt to reduce the complexity of the model. In doing so the models loss percentage was approaching 70%. I also attempted to add more neurons and hidden layers to the model, this action caused lower accuracy percentages.  

## Summary 

Based on my results I can conclude that adding more parameters to the model does not correlate with a higher accuracy percentage. Based on the model’s behavior, I can also conclude that dropping multiple columns does not correlate with a lower loss percentage, in fact, the loss percentage exponentially increased. With these results defining and creating a definitive list of features that must be tested would be a better option. Possibly creating sub datasets that test one to two features at a time or at the cost of accuracy, create one big dataset with must have features that need to be tested to find out if a applicant will achieve success. 
