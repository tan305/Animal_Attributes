# Predicting Animal Attributes using Convolutional Networks



   ![60ff98603b-emailer](https://user-images.githubusercontent.com/30891813/46539438-1a9e3d00-c8d4-11e8-926c-6311c9db90cd.jpg)

The dataset consisted of 12600 images of 50 different classes of animal. For every image the labelling of 85 attributes are provided and we needed to predict the same on the test dataset. You can download the dataset from [here](https://s3-ap-southeast-1.amazonaws.com/he-public-data/DL3%20Datasete37c45e.torrent)(Torrent Link).

Used Keras with TensorFlow backend for the code. An ensembled model of Inception V3 and ResNet models were used for final prediction.

To avoid overfitting we augment the images, it also helps us to train our model on a larger dataset making it more reliable. We perform the following augmentations,<br>
1. Rotate the images by not more than 20 degree.<br>
2. Shift the images slighty.<br>
3. Flip the images horizontally.<br>
4. Alter values of the RGB pixels of the images using customized function.<br>

Metrics used - F1 Score averaged over the 85 attributes<br>
Final score - The final F1 score is around **0.97**

Everything is implemented in Jupyter notebook which will hopefully make it easier to understand.

## Dependencies
- Keras 2.1.5
- Tensorflow 1.8.0
- Numpy
- Pandas
- Pickle
- Matplotlib
- PIL
- sklearn
