# Ageing Sign Detection Project

This project aims to detect signs of ageing in facial images using deep learning models. The project involves training a model using the EfficientNetB0 architecture and then using it to predict various ageing signs such as dark circles, puffiness, and wrinkles. The project also includes visualizing facial landmarks for detecting puffiness around the eyes.

## Project Overview
The project consists of two main parts:
1. **Ageing Sign Detection**: This part involves loading a pre-trained model, detecting faces in images, and predicting the presence of various ageing signs.
2. **Model Training**: This part involves training a model using the EfficientNetB0 architecture to classify facial images into different ageing sign categories.

## Features
- Detects various ageing signs in facial images such as dark circles, puffiness, and wrinkles.
- Visualizes facial landmarks for more accurate detection of puffiness around the eyes.
- Uses EfficientNetB0 architecture for training the model.
- Supports image augmentation to improve model robustness.

## Installation
To set up this project, you need to have the following dependencies installed:
- Keras
- TensorFlow
- OpenCV
- Dlib
- Imutils
- Numpy
- Matplotlib
- Scikit-learn

You can install these dependencies using pip:
```bash
pip install keras tensorflow opencv-python dlib imutils numpy matplotlib scikit-learn
```
## Usage

### Ageing Sign Detection

#### Load Model
Load the pre-trained model and weights:
```python
json_file = open("path to model.json file", "r")
loaded_model_json = json_file.read()
json_file.close()
loaded_model = model_from_json(loaded_model_json)
loaded_model.load_weights("path to weights.h5 file")
```

## Detect Signs
## Detect faces and predict ageing sign
```python
image = cv2.imread("path to image")
face_cascade = cv2.CascadeClassifier("path to cascade.xml file")
```
