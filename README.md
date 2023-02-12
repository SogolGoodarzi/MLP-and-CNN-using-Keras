# MLP-and-CNN-using-Keras
This Project has two main parts. The first part is about the implementation of MLP networks and the second part is about the implementation of CNN. 

### About the dataset
The given dataset is CIFAR10. The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.

Here are the classes in the dataset, as well as 10 random images from each:

![image](https://user-images.githubusercontent.com/125180530/218309897-969e66ca-f0ac-4684-a8f5-7c90cfcce0d6.png)

### Preprocessing the dataset
First of all, we need to normalize the data. It means that we divide each pixel of the train and test dataset to their maximum value which is 255. Then, we should divide the train dataset into train and validation. Around 5000 of the train data is assigned for the validation set. 

### 1) MLP
* For different ***batch sizes*** of 32, 64, and 128 we train the network and compare these three states regarding the accuracy and the time needed to train the network.

* Then we change the ***activation functions*** in each of the hidden layers of the network and evaluate the effect of different activation functions.

* Now it's time to evaluate the influence of ***loss function*** in the functionality of the network.

* For the ***optimizer***, there are different types that can be used. For example, Adam, Stochastic Gradient Descent (SGD), and so on. In this step, we change the optimizer to see the changes happening in the training process of the network. 

Now for improving the network we can use a combination of MLP and CNN. 

### 2) MLP + CNN
We have to add convolutional layers to the best achieved network in the previous part. Then, we make comparisons between the two implemented networks.

* Now we add ***pooling*** and ***batch normalization*** layers and evaluate the model regarding the accuracy and error of the network.

* Now it's time to add ***dropout*** and see if there is any change in the functionlaity of the network.

* The final improvement is to implement ***early stop*** concept and see its effect on the network.  
