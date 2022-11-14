# Udacity AI Programming with Python Project
## Create Your Own Image Classifier with Deep Learning with PyTorch


### I completed this project during 2020 summer holidays at [Udacity](https://udacity.com).

In this project I built a Python application that can train an image classifier on a flower dataset, then predict new images using the trained model. 

In addition to creating supporting files, I created two files ***train.py*** and ***predict.py***. 
1. ***train.py*** &nbsp; to train a new network on the flower dataset and save the model as a checkpoint.
   -  Prints out training loss, validation loss, and validation accuracy as the network trains
   -  Set hyperparameters as
````
    learning_rate = 0.01
    arch = 'vgg16'
    hidden_units = 200
    epochs = 30
````
  
1. ***predict.py***  &nbsp; uses a trained network to predict the class for an input image.
   - Predict flower name from an image and class probability.


#### Tools
As GitHub does not allow to upload files more than 100M size, I have split file "my_model.pth " of size 150M into the chunks of 50M as show below

```
 split -b 50m my_model.pth my_model_dot_pth.
```
If desired, we can combile 50M chunks of split files to get original "my_model.pth after cloning this repo
```
 cat my_model_dot_pth.?? > my_model.pth
```

<br />
<br />
<br />
References:

1. https://docs.python.org/3/library/argparse.html
2.	https://pymotw.com/3/argparse/







