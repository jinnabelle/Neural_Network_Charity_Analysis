# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:<br>
The purpose of this analysis is well defined (4 pt)<br>

In this analysis, I use Neural Networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Based on a dataset that has 34,000 rows of organization, we use information like section of industry and organization type to determine/predict whether an organization will be successful.

## Results:<br>
There is a bulleted list that answers all six questions (15 pt)<br>

Data Preprocessing<br>
What variable(s) are considered the target(s) for your model?<br>
The variable considered for the target is the is_successful field.

What variable(s) are considered to be the features for your model?<br>
Every field except for the target variable was considered to be features

What variable(s) are neither targets nor features, and should be removed from the input data?<br>
I dropped the first two fields which were EIN and NAME because they didn't provide any useful information for the data

Compiling, Training, and Evaluating the Model<br>
How many neurons, layers, and activation functions did you select for your neural network model, and why?<br>
There were two hidden layers for the neural network model, the first having 80 neurons and second layer having 30 neurons, and both layers having the relu activation. Output layer had sigmoid.

Were you able to achieve the target model performance?<br>
No, my model did not reach the target model performance. It had an accuracy of 59.7%
![Initial results](https://github.com/jinnabelle/Neural_Network_Charity_Analysis/blob/main/Initial%20Attempt.png?raw=true)


What steps did you take to try and increase model performance?<br>
I attempted three more times. Below are the approach I took for each attempt <br>

Attempt 1: 
I changed the second layer to have 40 neurons instead of the initial 30. The accuracy for this was 42% which was the lowest of the three attempts.
![Attemp1](https://github.com/jinnabelle/Neural_Network_Charity_Analysis/blob/main/Attempt1.png?raw=true)

Attempt 2: 
I added a third layer and changed the neurons for each layer. Layer 1 had 100 neurons, layer 2 had 50 and layer 3 had 20. The accuracy for this was 53.3%
![Attempt2](https://github.com/jinnabelle/Neural_Network_Charity_Analysis/blob/main/Attempt2.png)

Attempt 3: 
I kept the same amount of layers as the second attempt and changed the number of neurons for each layer with 80,70,30 neurons, respectively. I also changed the activation for the outer layer to tanh. The accuracy for this was 55%. 
![Attempt3](https://github.com/jinnabelle/Neural_Network_Charity_Analysis/blob/main/Attempt3.png)

## Summary:<br>
There is a summary of the results (2 pt)<br>

The model ended up having a lower accuracy than the initial attempt and this is due to overfitting. I think that if tweaked the features included it might have resulted differently.<br>
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)<br>
Another model might work better for classifying like the Random Forest model for a more accurate classifier. Random Forest classifier averages the dataset to improve the classify prediction and controls for overfitting.

