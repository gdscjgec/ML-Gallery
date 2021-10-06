# Artificial Neural Netwrok Vs. Convolutional Nural Network !! [Image Classification]

## Notebook :

  [Notebook](https://colab.research.google.com/drive/1cIIXFeROtJf7MovU7j6ipBDvur-X1o9M?usp=sharing)
  
## Dataset :

  [**CIFAR-10**](https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz). (In this project the dataset has been directly loaded from the Tensorflow datasets :
    ```
    tensorflow.keras.datasets.cifar10.load_data()
    ```
  The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.
  
## Models :

  * ***Net-A*** - A single layer perceptron with 10 outputs without any hidden layer
     ```
     _________________________________________________________________
      Layer (type)                 Output Shape              Param #   
      =================================================================
      flatten_13 (Flatten)         (None, 3072)              0         
      _________________________________________________________________
      dense_23 (Dense)             (None, 10)                30730     
      =================================================================
        Total params: 30,730
        Trainable params: 30,730
        Non-trainable params: 0
      ```  
  * ***Net-B*** - Neural network with slightly more complication , that is , it has a hidden layer with 300 nodes and adds a non-linearity between the layers.
    ```
    _________________________________________________________________
    Layer (type)                 Output Shape              Param #   
    =================================================================
    flatten_14 (Flatten)         (None, 3072)              0         
    _________________________________________________________________
    dense_24 (Dense)             (None, 300)               921900    
    _________________________________________________________________
    dense_25 (Dense)             (None, 10)                3010      
    =================================================================
      Total params: 924,910
      Trainable params: 924,910
      Non-trainable params: 0
    ```
   
  * ***Net-C*** - A Convolutional Neural Network with one convolution layer , with 32 filtres of size 5x5 , with padding and activation function set to "relu". It is followed by                   a Max-pooling layer of size (2,2) with strides=2.Then after flattenning , a dense layer of 512 nodes is added before the final output layer with "softmax"                         activation.   
    ```
    _________________________________________________________________
    Layer (type)                 Output Shape              Param #   
    =================================================================
    conv2d_9 (Conv2D)            (None, 32, 32, 32)        2432      
    _________________________________________________________________
    max_pooling2d_9 (MaxPooling2 (None, 16, 16, 32)        0         
    _________________________________________________________________
    flatten_15 (Flatten)         (None, 8192)              0         
    _________________________________________________________________
    dense_26 (Dense)             (None, 512)               4194816    
    _________________________________________________________________
    dense_27 (Dense)             (None, 10)                5130       
    =================================================================
      Total params: 4,202,378
      Trainable params: 4,202,378
      Non-trainable params: 0
    ```
    
    * ***Net-D*** -A Convolutional Neural Network with two convolution layer , first one with 32 filters of size 5x5 , with padding and activation function set to "relu". It is followed by               a Max-pooling layer of size (2,2) with strides=2. Then a second convolution layer with 64 filters of size 4x4 and activation function set to "relu". It is followed by    
                   a Max-pooling layer of size (2,2) with strides=2.It is followed by a Dropout layer of size (0.2). Then after flattenning, a dense layer of 512 nodes is added before the final output layer with "softmax" activation.
      ```
    _________________________________________________________________
    Layer (type)                 Output Shape              Param #   
    =================================================================
    conv2d_19 (Conv2D)           (None, 32, 32, 32)        2432      
    _________________________________________________________________
    max_pooling2d_19 (MaxPooling (None, 16, 16, 32)        0         
    _________________________________________________________________
    conv2d_20 (Conv2D)           (None, 13, 13, 64)        32832     
    _________________________________________________________________
    max_pooling2d_20 (MaxPooling (None, 6, 6, 64)          0         
    _________________________________________________________________
    dropout_6 (Dropout)          (None, 6, 6, 64)          0         
    _________________________________________________________________
    flatten_18 (Flatten)         (None, 2304)              0         
    _________________________________________________________________
    dense_32 (Dense)             (None, 512)               1180160   
    _________________________________________________________________
    dense_33 (Dense)             (None, 10)                5130      
    =================================================================
      Total params: 1,220,554
      Trainable params: 1,220,554
      Non-trainable params: 0
      
## Visualisation :

   A visualization of all the results with respect to the images and their classes are done , which gives an idea of the performance of each of the networks.
   
## Results :

   Each of the networks are iterated through 50 epochs.
   Test accuracy of the networks are given below:
```
    Test accuracy of NetA-  10.39000004529953 %    
    Test accuracy of NetB-  47.360000014305115 %
    Test accuracy of NetC-  64.38000202178955 %
    Test accuracy of NetD-  70.1200008392334 %
```   
