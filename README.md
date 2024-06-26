# Image Classification Training with tensorflow

This is an image classification project that trains a model to classify types of apparel using tensorflow.

Classifies the following images in the folder(imgDataSet):
- Boys Apparel
- Girls Apparel
- Mens Footwear
- Womens Footwear
<br>

The dataset is not mine. -> https://www.kaggle.com/datasets/vikashrajluhaniwal/fashion-images

## Setting up your environment
```
pip install -r requirements.txt
```

The two libraries used are tensorflow and opencv. So if you are trying to run this from google colab or jupyter notebook then just:
```
pip install tensorflow
pip install opencv-python
```

## Training the model 
The current model "object_detection_v1.h5" has an accuracy of 81% and is trained using train.py . You can train your own model by changing the layers and nodes of the neural network in train.py.
```
python train.py
```

## Predicting from the model
There are two ways to run the prediction script.
- This will predict all the images in the "google_images_for_external_testing" folder you can add more images into that folder.
```
python predict.py 
```
- This will predict any image you give it.
```
python predict.py <path_of_your_custom_image>
```
