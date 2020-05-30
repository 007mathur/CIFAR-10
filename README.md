# CIFAR-10<br>
This repository is a comparative study of three most basic models in the field of Computer Vision, i.e., Neural Networks, Convolutional Neural Networks, and Residual Neural Networks.<br>

## DataSet<br>
These models were trained on training data of 50000 images and tested on data 10000 images available as built-in datasets in [Keras](https://keras.io/api/datasets/cifar10/).<br>
These images were of the size 32*32*3 and they could be mutually exclusively classified into 10 classes. The labeled classes in the datasets are:
- Airplane 
- Automobile 
- Bird 
- Cat 
- Deer 
- Dog 
- Frog 
- horse 
- Ship 
- Truck

## [Neural Network](https://github.com/utmaktharsurh/CIFAR-10/blob/master/nn.ipynb)<br>
The architecture of neuralnetworks consists of 3 hidden layers of 784, 84, and 20 units. A batch normalisation layer is added in between the 2nd and the 3rd hidden layer.<br>
The Model has 2,477,418 parameters out of which 2,447,250 parameters are trainable and rest 168 parameters are non-trainable. Atfer training the model over 15 epochs in batch sizes of 256 (196 batches per epoch), it is able to achieve an accuracy of 43.67%.<br>

## [Convolutional Neural Networks](https://github.com/utmaktharsurh/CIFAR-10/blob/master/cnn.ipynb)<br>
The architecture of neuralnetworks consists of 3 convolution blocks and a fully connected layer of 32 units.<br> 
A convolutional block consists of a convolutional layer followed by a max pooling layer. The number of channels after convolution blocks are 6, 16, and 32 respectively. A batch normalisation layer is added after every convolutional block and the fully connected layer.<br>
The Model 22,778 parameters out of which 22,606 parameters are trainnable and rest 172 parameters are non-trainable. After training the model over 20 epochs in batch sizes of 256 (196 batches per epoch), it is able to achieve an accuracy of 67.39%.<br>

## [Residual Neural Networks](https://github.com/utmaktharsurh/CIFAR-10/blob/master/resnet.ipynb)<br>
The architecture of neuralnetworks consists of 4 convolution blocks and a fully connected layer of 32 units.<br> 
The number of channels after convolution blocks are 6, 16, 32, and 64 respectively. A batch normalisation layer is added after every two convolutional block and the fully connected layer.<br>
The Model 39,144 parameters out of which 38,920 parameters are trainnable and rest 224 parameters are non-trainable. After training the model over 20 epochs in batch sizes of 256 (196 batches per epoch), it is able to achieve an accuracy of 69.26%.<br>

**By this comparative study I've observed that by using the concept of residual networks or skip connections, accuracy of a Computer Vision Model can be enhanced.**<br>

If you've any suggestions or feedbacks, please feel free to drop comments and make pull requests.
