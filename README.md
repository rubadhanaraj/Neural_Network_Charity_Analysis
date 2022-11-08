# Neural_Network_Charity_Analysis
## Overview 
The purpose of this project is to explore and implement neural networks using the TensorFlow platform in Python. The major costs and benefits of different neural networks were discussed and these costs have been compared to traditional machine learning classification and regression models. Also,implementing neural networks and deep neural networks across a number of different datasets, including image, natural language, and numerical datasets have been practised. The main objectives were to
* Compare the differences between the traditional machine learning classification and regression models and the neural network models.
* Describe the perceptron model and its components.
* Implement neural network models using TensorFlow.
* Explain how different neural network structures change algorithm performance.
* Preprocess and construct datasets for neural network models.
* Compare the differences between neural network models and deep neural networks.
* Implement deep neural network models using TensorFlow.
Using the features in the provided dataset from Alphabet Soup, a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup was created. Alphabet Soup’s dataset (CSV) had more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Results
### Data Preprocessing for a neural network model
1. In the given dataset, "IS SUCCESSFUL" column was considered as target as this column is a binary classifier that is capable of predicting whether applicants          will be successful if funded by Alphabet Soup.
2. The variables which were considered as features were, "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT",        "SPECIAL_CONSIDERATIONS", "ASK_AMT".
3. "EIN" and "NAME" columns were considered neither as targets nor as features. All the categorical variables have been encoded,standardized and split into              training and testing data.
 
### Compiling, Training, and Evaluating the Model
1. The deep-learning neural network model has two hidden layers with 80 and 30 neurons each with the activation functions ReLu. The output layer has a single neuron with sigmoid activation function as it is a binary classifier. 

![image](https://user-images.githubusercontent.com/108298416/200475279-59483399-2183-4d23-9281-27690a0847d7.png)

2. The accuracy for the model acheived through deep-learning neural network is 72.6%. However the target predictive accuracy was supposed to be 75%

![image](https://user-images.githubusercontent.com/108298416/200475700-ea029191-5a8b-4750-b801-2dea0f533b9d.png)

3. To optimise and increase the model performance, the columns "STATUS" and "SPECIAL_CONSIDERATIONS" were dropped, more hidden layers were added, more neurons were added to each hidden layer and the activation function for each hidden layer is changed.In first attempt, the numbers of neurons in the hidden layers were increased to 100 and 30. In the second attempt the thrid hidden layer was added and then the activation functions have been changed in the third attempt. But the model's accuracy didn't change much even after optimising the model. 

![image](https://user-images.githubusercontent.com/108298416/200477770-b7576541-9fef-4288-9c8d-6186913f7d1e.png)

![image](https://user-images.githubusercontent.com/108298416/200477867-48f48f15-1f5d-4f7f-8ec2-f8ce33aa2be6.png)

## Summary
The overall results of the deep learning model shows that the accuracy of the model is 72.7% after optimization, though the target predicitve accuracy was 75%. As this is a binary classification model, supervised machine learning models such as Random Forest classifier model can be used to generate the results and the performance can be compared against deep learning neural network model.

