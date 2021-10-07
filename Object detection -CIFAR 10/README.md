# Object Detection Model
# Dataset :

[CIFAR 10](https://www.cs.toronto.edu/~kriz/cifar.html) 

# Models: 

We use 2 different object detection models to classify the dataset. The given dataset has multiple tiny images of objects features. There are 60000 images totally, the neural networks we select classify the objects based on the characteristic features of an object . 

The Project Uses 2 different object detection models, namely

1. Artificial Neural Networks
2. Convoluted Neural Networks

# Results:

Here are the accuracy rates seen by implementing differet models 
  |Model              |Accuracy         |
  |:-----------------:|:---------------:|
  |ANN                |47%              |
  |CNN                |65%              |


# Test Accuracy For the Model

Test_acc = 0.48 for ANN after 5 epochs
test_acc = 0.67 for CNN after 5 epochs
  
5 epochs give us 67 percent accuracy, implies more epochs can give us even more accuracy. We add 2 maxpooling layers, and 2 dense layers, increasing our neural network may increase the accuracy

