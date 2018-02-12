# Project 5 - Vehicle Detection
## 1 Training a Classifier

### 1.1 Download the Data Set
Data sets for [vehicle](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/vehicles.zip) and [non-vehicle](https://s3.amazonaws.com/udacity-sdc/Vehicle_Tracking/non-vehicles.zip) were downloaded to train the classifier with. Below are some examples of images with and without cars and varying ranges of resolution. The more images provided, the better your classifier will be.

<p align="center">
 <img src="./res/images/data_set.png" width=550>
</p>

### 1.2 Extract Features
Images contain many sets of features that can be extracted to help our classifier identify whether there is a vehicle in the image or not. Several methods for feature extraction include abstracting an image into a histogram of colours and a histogram of oriented gradients (HOG). 

<p align="center">
 <img src="./res/images/hog_feature.png" width=550>
</p>

Parameters such as color space (RGB/HSV/LUV), number of bins, and number of gradient orientations can be fine tuned to further increase the performance of the classifier. Combining multiple methods is ideal however the magnitudes of the features have to be normalized so that one type of feature doesn't overruled another.

<p align="center">
 <img src="./res/images/normalize_data.png" width=550>
</p>

### 1.3 Label Data Set
With the ability to extract features from images, we need to apply labels to the images inorder to allow the classifier to categorize the images. For this project the labels are simple: '1' for car and '0' for not car. Note: ensure that the relative sizes of the data sets are fairly equal in size to ensure that the classifier will not favour one type of image over the other.

### 1.4 Build the Classifier
The labelled data set was shuffled and 20% of the images extracted to create a training and testing set for evaluating the classifier. From the Python Scikit-Learn I used the LinearSVC.

## 2 Searching for Vehilces
### 2.1 Sliding Window Approach
...

### 2.2 Heat Mapping
...

<p align="center">
 <img src="./res/images/heatmap.png" width=550>
</p>

### 2.3 Vehicle Tracking between Frames
...

## 3 Pipeline (Image)
...


## Pipeline (Video)
...





 


