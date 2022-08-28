# Image-Caption-Generator-Using-Deep-Learning---VGG19-ResNet50-InceptionV3
Generate caption for images

Introduction

Image caption generator is a process of recognizing the context of an image and annotating it with relevant captions using deep learning, and computer vision. It includes the labeling of an image with keywords with the help of datasets provided during model training. For this project, Flicker8k dataset is used to train the CNN models (VGG19, ResNet50, and Xceptions). The three pretrained models are used for image feature extraction. The extracted features are fed to the LSTM model which in turn generates the image caption. BLEU score is used to evaluate model performance. The performance of the three models are compared.

Dataset:

1. Flicker8k image dataset
3. Captions text file
Path: https://www.kaggle.com/datasets/ming666/flicker8k-dataset

Pre-trained models:
  VGG19
  ResNet50
  Inception_V3

Pre-requisites

I use Google colab notebook to run this caption generator. The first notebook is to train the CNN models, and the sencond notebook is to generate captions for new images using streamlit in google colab. The google colab notebooks are used because Tensorflow and Keras are readily available. You can run it in Jupyter notebook or other IDEs if you install tensorflow and Keras. 

Steps to train CNN model/models:

Section I 

1. Load captions with image IDs
2. Preprocess the captions: 1) convert to lowercase, 2) remove digits and special characters, 3) remove additional spaces, 4) add begin and end tags to the caption 
3. Tokenize the captions (text data)

Section II

1. Load images 
2. Extract image features:
      a. Load pre-trained models (VGG19, ResNet50, InterceptV3) with weights = 'imagenet' 
      b. Save extraced features
 
 Section III 
 
 1. Train models
 2. Define Caption Generation Models 
 3. Save models 

Section IV

1. Evaluate caption generation model performance using BLEU Score 

Section V

1. Predict/generate captions for images 


Section VI  Deployment 



 
 
