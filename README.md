# AlphabetSoup_Analysis

#### Data Preprocessing
----
1. What variable(s) are considered the target for your model?
Is-Successful
---
2. What variable(s) are considered to be the features for your model?
ANSWER: The features of this model are the NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT,SPECIAL_CONSIDERATIONS, STATUS, and ASK_AMT
---
3. What variable(s) are neither and should be removed from the input data? 
ANSWER:  EIN (Employer identificaiton) was dropped because the numbers could confuse the system into thinking its significant.
ANSWER: A student could drop SPECIAL_CONSIDERATIONS because there is only a small percentage of cases that had any special consideration, and special considerations cannot be quantified.
ANSWER: A student could drop STATUS because  all rows were the same value, 1.
Compiling, Training, and Evaluating the Model
How many neurons, layers, and and activation functions did you select for your neural network model, and why? ANSWER: In this model there are three hidden layers each with many neurons, because this seeemed to increased the accuracy above 75%. The number of epochs wasn't changed. The first activation function was 'relu' but the 2nd and 3rd were 'sigmoid'and the output function was 'sigmoid'. Changing the 2nd and 3rd activation functions to 'sigmoid' also helped boost the accuracy.
Were you able to achieve the target model performance? ANSWER: Yes
What steps did you take to try and increase model performance? ANSWER: It required converting the NAME column into data points, which has the biggest impact on improving efficiency. And, it also required adding a third layer and using the "sigmoid" activation function for the 2nd and 3rd layer.
