# Mnist
It’s a dataset of classified handwritten images in a 28 x 28 format.      
60,000 training images     
10,000 testing images
I was able to build a classifier that was able to detect the test set with an accuracy of ~99%. It took about 15 minutes to train on my Laptop.



I have build a CNN with the following architecture, using Keras’ Sequential API:

    #3 Conv2D layers with 32, 64 and 64 filters each, using the relu activation, kernel_size=(3,3) and padding=’same’
    #Each Conv2D layer is followed immediately by a MaxPooling2D layer with a pool_size=(2,2)
    #Followed with a Dense layer with 512 nodes and relu activation
    #Finally, the output layer is a Dense layer with 10 nodes (corresponding to the 10 output classes) and softmax activation function — we use  softmax for multi-class classification
