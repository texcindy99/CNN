### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

You need to install TensorFlow to run the code here besides the Anaconda distribution of Python.

Note that you need to download two sets of data before running the code.

1. Download the dataset of dog images [here](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip) and place it in the respository.
2. Download the output of dog images passing through the pretrained VGG-16 network [here](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) and place it in the bottleneck_features/ folder.

## Project Motivation <a name="motivation"></a>

This is the image classification project using CNN. I was interestested in using pretrained VGG-16 network for ImageNet competition to classify the dog breed using dog images in my data base using the following steps:

1. Loading the data which is the output of dog images passing through the pretrained network, stopping at the last VGG-16 max pooling layer;
2. Slice off the end of VGG-16 network and add a new classification layer with 133 nodes;
3. Only training weights in the new layer and freeze the weights in other layers because the dog image set is relative small and has significant overlap with subset of ImageNet category.

## File Descriptions <a name="files"></a>

There is one notebook available here to showcase work related to the above questions. The notebook is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.  

There are ... data files used in the notebook. "..." is the data file for... .

The data file is available at [website](http://....).

## Results <a name="results"></a>

The main findings of the code is ....

## Licensing, Authors, Acknowledgements <a name="licensing"></a>

Must give credit to .... for the data.  You can find the Licensing for the data and other descriptive information at the link available [here](http://...).  Otherwise, feel free to use the code here as you would like! 
