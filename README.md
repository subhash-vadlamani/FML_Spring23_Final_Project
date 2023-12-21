# Final Project - AIXPERTS

<!-- ABOUT THE PROJECT -->
## About The Project

These Jupyter notebooks includes the necessary training and test functions to create a neural network model using the ResNet50V2 architecture, which is then trained on a given dataset of images. The model is designed to classify images into one of ten categories using the sparse categorical cross-entropy loss function and the Adam optimizer. It also has the capability to classify unknown classes by passing a certain parameter in the test function.

## Dependencies

Please ensure that the following libraries are installed before running the scripts: 

1. numpy

2. tensorflow 2.7.0

3. keras

4. scikit-learn

## Usage

Put the .npy files for the training/testing data and labels in the same directory as the train and test notebooks.
Our model file (AIXPERTS_Final_model.h5) was turned in on Canvas in a zip folder. Please extract those weights into the directory containing the test script for the testing process. The test script is already configured to test those weights.

### Training Script - train.ipynb

This notebook contains the model architecture and function to create the CNN. To use, run "train(data, labels, model)" where data is the filename of the file containing the training data and labels is the filename of the filename containing the associated labels. Make sure to include quotations around the filenames.

This function saves the best weights in a file called "model.h5".

### Test Script - test.ipynb

This notebook contains the script to test the accuracy of the model we provided, in the file "AIXPERTS_Final_model.h5".

**For model performance on the easy test set**

Run "test(test_data, test_labels, hard=False)", where test_data is the filename of the file containing the testing data, test_labels is the filename of the file containing the associated labels, and hard = False will return the accuracy and predictions for classification of the 10 classes. Make sure to include quotations around the filenames.

## Extra credit problem

**For model performance on the hard test set**

Run "test(test_data, test_labels, hard=True)", where test_data is the filename of the file containing the testing data, test_labels is the filename of the file containing the associated labels, and hard = True will return the accuracy and predictions for classification of both the 10 classes and the unknown class(-1).  Make sure to include quotations around the filenames.
