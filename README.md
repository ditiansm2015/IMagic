# IMagic
Coloring of image using Artificial Neural Network

1. IMagic-Training: This python notebook is used to train the model<br>
2. IMagic-Output: This python notebook is used to predict the output


IMagic is a Machine Learning based model to color a black and white image i.e. by converting a Grayscale image into RGB image


**About Dataset**

The datasets are image files that can be read using the open-cv python library. Each sample image used was originally 256x256 pixels and consists of 3 bands - red, green, and blue. These images are resized into 64x64 pixels images and converted separately into Grayscale image which could be used as input and original 3 bands image as an output to neural network.

The dataset comprises 721 RGB images that have been converted into Grayscale for the purpose of training and testing



**Methodology**

This model follows the methodology of Supervised Learning using Regression where we have to predict a particular value for input features.

Neural network used for converting grayscale image to RGB image takes a 64X64 pixels grayscale image as input and 64x64x3 pixels RGB image as an output. These images are converted into single vertor before feeding into the neural network. Then model is trained over these images repeatedly to achieve the minimal loss and highest accuracy.



**Steps**

1. Aim - to Convert a Grayscale image to RGB Image 
2. Converted 256*256*3 pixels RGB images into 64*64 pixels grayscale images and converted into single vector for training Artificial Neural Network model
3. Created placeholder to pass Training Data
4. Trained the tensorflow based neural network with the gathered data.
5. Created batches for training the model
6. Saved the parameters as h5py file
7. Read the parameters file and performed similar steps for printing the RBG converted images which was of the size 64*64*3 (one pixel each for Red, Green and Blue colours) 
8. The accuracy on training dataset was 77% (approx.) and 53%(approx.) on test dataset.
