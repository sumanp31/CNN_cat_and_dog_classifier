# CNN_cat_and_dog_classifier

## Data Preprocessing

1. All pixel are rescalled to be between (1,255)
2. All images are resized to (128,128)

## Network Description

1. There are 3 sets of convolution and maxpool layers.

    **a.** First convolution layer has 32 filters of size (3,3) and uses RELU    activation, followed by a maxpooling layer of size (2,2).
     
     **b.**  Second convolution layer has 64 filters of size (3,3) and uses RELU    activation, followed by a maxpooling layer of size (2,2).
     
     **c.**  Third convolution layer has 32 filters of size (3,3) and uses RELU    activation, followed by a maxpooling layer of size (2,2)
     
2. Followed by 2 fully connected layer.

	**a.** The first fully connected layer has 128 activation unit and has a RELU activation function. The output of previous layer is flattened and is passed as input to this layer.

	**b.**  The first fully connected layer has 128 activation unit and has a Sigmoid activation function.


## Experiment
- The dataset has 10000 pics. 5000 of each cats and dogs. The dataset is split into training and test set in the ratio 8:2.
- The Experiment was run for 25 epochs.
- The batch size is 16.

## Output
The prediction worked for the couple of single image prediction made.
![ ](https://github.com/sumanp31/CNN_cat_and_dog_classifier/blob/master/result1.png  "Consol Output")

It can be seen from the consol output that the final output has a training set accuracy of 99% and validation set accuracy of 85%.
I am still working on the overfitting.
