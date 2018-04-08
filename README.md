#facerecognition-NeuralNet

This is a project i'm making for the school subject "Introduction to 
Scientific Programming".

###Overview

The project is just a Neural Net, which is done in Python using 
Jupyter Notebook which aims to recognice faces of 2 different persons 
(in this case Japanese models), being trained with pictures of the faces 
and a vector that tells the Neural Net when training which person 
was of the input picture.

Then it's tested by passing any picture of these persons and getting an 
output from the net (which is the Name, a prediction)


###Method

A Neural Net with 3 hidden layers is used, getting the input neurons 
from the pictures (at first each pixel from the picture, which isn't 
optimal, later as features are identified and extracted, they will be 
used to optimize the process), each hidden layer has the same number of 
neurons as the input layer, and the output layer has 2 neurons (if we 
want to classify faces from more persons, we increase the output layer 
by 1 neuron for each person we are adding).

The training method is as usual: Feed-forward and back-propagation using 
as activation function a sigmoid function (1/(1+e^-x)) for 
updating weights, so we can later on test the Net with different 
pictures.

The Neural Net is done in a class, so one can just use create an 
instance of the class (a Neural Net Object) and use its methods to train 
or test.

###Comments

The comments are in spanish because i need my grade for school :P
