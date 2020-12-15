# CIFAR-10<br>
This repository is a comparative study of three most basic models in the field of Computer Vision, i.e., Neural Networks, Convolutional Neural Networks, and Residual Neural Networks.<br>

## DataSet<br>
These models were trained on training data of 50000 images and tested on data 10000 images available as built-in datasets in [Keras](https://keras.io/api/datasets/cifar10/).<br>
These images were of the size 32x32x3 and they could be mutually exclusively classified into 10 classes. The labeled classes in the datasets are:
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
The architecture of neural networks consists of 2 hidden layers of 784, and 100 units. A batch normalisation layer is added in between the 2nd and the 3rd hidden layer.<br>
The Model has 2,492,278 parameters out of which 2,490,510 parameters are trainable and rest 1,768 parameters are non-trainable. Atfer training the model over 15 epochs in batch sizes of 128 (391 batches per epoch), it is able to achieve an accuracy of 48.42%.<br>

## [Convolutional Neural Networks](https://github.com/utmaktharsurh/CIFAR-10/blob/master/cnn.ipynb)<br>
The architecture of neural networks consists of 3 convolution blocks and a fully connected layer of 100 units.<br> 
A convolutional block consists of a convolutional layer followed by a max pooling layer. The number of channels after convolution blocks are 16, 32, and 64 respectively. A batch normalisation layer is added after every convolutional block and the fully connected layer.<br>
The Model 127,942 parameters out of which 127,518 parameters are trainnable and rest 424 parameters are non-trainable. After training the model over 20 epochs in batch sizes of 128 (391 batches per epoch), it is able to achieve an accuracy of 72.899%.<br>

## [Residual Neural Networks](https://github.com/utmaktharsurh/CIFAR-10/blob/master/resnet.ipynb)<br>
The architecture of neural networks consists of a convolutional layer, 4 convolution blocks and a fully connected layer of 200 units.<br> 
The number of channels after convolution blocks are 16, 32, 63, and 128 respectively. A batch normalisation layer is added after every two convolutional block and the fully connected layer.<br>
The Model 540,820 parameters out of which 539,926 parameters are trainnable and rest 894 parameters are non-trainable. After training the model over 20 epochs in batch sizes of 64 (782 batches per epoch), it is able to achieve an accuracy of 77.759%.<br>
<br>
| Model                              | Accuracy | Loss  |
| :--------------------------------: | :------: | :---: |
| Neural Network Model               | 48.42%   | 1.488 |
| Convolutional Neural Network Model | 72.899%  | 1.555 |
| Residual Neural Network Model      | 77.759%  | 1.289 |


**By this comparative study I've observed that by using the concept of residual networks or skip connections, accuracy of a Computer Vision Model can be enhanced.**<br>

If you've any suggestions or feedbacks, please feel free to drop comments and make pull requests.
