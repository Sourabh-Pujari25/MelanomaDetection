# Melanoma Detection Assignment
> In this assignment, I have build a multiclass classification model using a custom convolutional neural network in tensorflow.



## Problem Statement
* To build a multiclass classification model using a custom convolutional neural network in TensorFlow. To build a CNN based model which can accurately detect melanoma a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that 
<!-- You can include any other section that is pertinent to your problem -->

## General Information About the Data
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- Keras
- TensorFlow
- Python 3
- Pandas, Numpy, Matplotlib,
- Augmento

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

#### Accuracy and Loss for model 1
- Accuracy and Loss for model 1

#### Model 1 
- Trained for 20 epochs with available data
- Observations:
- The model clearly overfits.
- The training accuracy is continuously increasing while the validation accuracy is fluctuating around 50%.
- The loss on training set decreases after each epoch but in case of the validation loss, its increasing after decreasing for few initial epochs.
- The model memorized the data instead of generalizing and learning real features and general relationships.


#### Model 2 was trained for 20 epochs with keras built-in data augmentation.
- Following augmentations were used
- Rotation
- Zoom
- Flip - vertical and horizontal
- Observations:
- The application of data augmentation and dropout layer reduced overfitting.
- Results on training and validation datasets are much closer.
- Overall accuracy is not high.

#### Model 3
- Accuracy and Loss for model 3 - Class imbalance changes + Dropout and Batch Normalization
- Accuracy and Loss for model 3 - Class imbalance changes + Dropout


#### Model 3 was trained for 30 epochs
- Augmentor was used to reduce class imbalance (500 images per class got added)
- Observations:
- Changes done for data imbalance helped in improving training and validation accuracy.
- On top of data imbalance changes, tried two options
- With dropout and batch normalization
- With only dropout
- Out of two models, we can observe that training and validation accuracy are better in-sync in case of only dropout model
Even though validation accuracy increased when compared with 1st and 2nd models, still there is 0.1 gap between training and validation accuracy.


# References
- https://keras.io/guides/
- https://towardsdatascience.com/
- https://www.tensorflow.org/tutorials/images/data_augmentation
- https://augmentor.readthedocs.io/en/stable/





<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
