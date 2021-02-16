# Predicting Animal Attributes using Convolutional Networks

   ![60ff98603b-emailer](https://user-images.githubusercontent.com/30891813/46539438-1a9e3d00-c8d4-11e8-926c-6311c9db90cd.jpg)

## Problem Statement
Currently, animal detection and recognition are still a difficult challenge and there is no unique method that provides a robust and efficient solution to all situations. Generally, features from the animal that belongs to a certain class are used to train a certain classifier. Then, given a new input image, the classifier will be able to decide if the sample is the animal or not. To better understand the complexities of natural ecosystems and better manage and better protect them, it would be helpful if we can differentiate the animals based on their attributes and characteristics.

In this task, 18000 images of 50 animals classes with pre-extracted feature representation for each image. The classes are aligned with Osherson’s classical class/attribute matrix, thereby providing 85 numeric attribute values for each class.

Given the image of an animal, the task is to identify all the characteristics/ attributes associated with that animal.You can download the dataset from [here](https://s3-ap-southeast-1.amazonaws.com/he-public-data/DL3%20Datasete37c45e.torrent)(Torrent Link).

Used Keras with TensorFlow backend for the code. An ensembled model of Inception V3 and ResNet models were used for final prediction.

To avoid overfitting we augment the images, it also helps us to train our model on a larger dataset making it more reliable. We perform the following augmentations,<br>
1. Rotate the images by not more than 20 degree.<br>
2. Shift the images slighty.<br>
3. Flip the images horizontally.<br>
4. Alter values of the RGB pixels of the images using customized function.<br>

Metrics used - F1 Score averaged over the 85 attributes<br>
Final score - The final F1 score is around **0.97**


## Dependencies
- Keras 2.1.5
- Tensorflow 1.8.0
- Numpy
- Pandas
- Pickle
- Matplotlib
- PIL
- sklearn
