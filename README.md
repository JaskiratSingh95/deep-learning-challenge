# deep-learning-challenge
Deploying Deep Learning
Question 1.
What variable(s) are the target(s) for your model? 
For this challenge, “IS_SUCCESSFUL” variable is the target in the model.

Question 2. 
What variable(s) are the features for your model? ? For this dataframe, the rest of the data, excluding “EIN” and “NAME” will be used as the features of the model: 
1 APPLICATION_TYPE, 
2 AFFILIATION, 
3 CLASSIFICATION, 
4 USE_CASE, 
5 ORGANIZATION, 
6 STATUS, 
7 INCOME_AMT, 
8 SPECIAL_CONSIDERATIONS, 
9 ASK_AMT.

Question 3
What variable(s) should be removed from the input data because they are neither targets nor features? For modelleing purposes, I am removing “EIN” and “NAME” as these are basically an identification column.

Question 4
How many neurons, layers, and activation functions did you select for your neural network model, and why?
The number of neurons in a dense layer of a neural network model determines the capacity of the network to learn complex patterns. More neurons allow the network to capture intricate relationships but can also lead to overfitting.
In this model challenge, I have used have different numbers of neurons in each layer in a decreasing order: 70, 30, 10, and 1. I considered the following factors for selecting my neuron range:
1 the size of your dataset,
2 the complexity of the task, 
The depth of the neural network (i.e., the number of hidden layers) impacts its ability to learn hierarchical features and affects it performance. My model has four layers: 
input, 
two hidden, 
output. 
The choice of layers depends on the problem and data. I avoided adding more layers as too many layers can lead to overfitting of the model. 
Activation functions introduce non-linearity to the model, allowing it to learn complex mappings for the model in question. I’ve used the ReLU (Rectified Linear Unit) activation function, which is common for hidden layers. It helps mitigate the vanishing gradient problem.
The softmax activation which I have used in the output layer is suitable for multi-class classification tasks.
