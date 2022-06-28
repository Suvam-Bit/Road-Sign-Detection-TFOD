# Road-Sign-Detection-TFOD

## Dataset URL
https://www.kaggle.com/datasets/andrewmvd/road-sign-detection

## Problem Statement

Object Detection on different road signs using Tensorflow Object Detection (TFOD)

## About Data
This dataset contains 877 images of 4 distinct classes for the objective of road sign detection.
Bounding box annotations are provided in the PASCAL VOC format
The classes are:

- Trafic Light
- Stop
- Speedlimit
- Crosswalk

## Analysis
1. The analysis has been done on `Google Colab Environment`
    - Model Training has been done on the notebook `TFOD_RoadSign_Train_The_Model.ipynb`
    - Model Inferencing has been done on the notebook `TFOD_RoadSign_Using_Pretrained_Model.ipynb`


2. Train Test Split
    - Number of train images: 789
    - Number of test images: 88


3. Download the pretrained model from the Tensorflow Models Zoo
    - Model: SSD MobileNet V2 FPNLite 320X320
    - Tensorflow Models Zoo: https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md


4. Clone the Git Repository of Tensorflow Models
    -  Tensorflow Models: https://github.com/tensorflow/models


5. Install Tensorflow Object Detection (TFOD) Module in the Colab Environment


6. Create the Label Map
    - For 4 classes: (i) Crosswalk (ii) Speedlimit (iii) Stop (iv) Traffic Light
    
    
7. Create the TFRecord file for training and testing


8. Update the model config as per our problem statement.


9. Train the Model
    - Number of training steps: 20000
    

10. Evaluate the Model
    - mAP: 0.568070
    - mAR: 0.562572


## Result:

NOTE: Our model did not performed well in detecting the 'stop' signs. It may be because there is a very less number of 'stop' sign samples in the dataset.

![alt text](https://github.com/Suvam-Bit/Road-Sign-Detection-TFOD/blob/main/sample_outputs/output_06.jpg?raw=true)
![alt text](https://github.com/Suvam-Bit/Road-Sign-Detection-TFOD/blob/main/sample_outputs/output_09.jpg?raw=true)
![alt text](https://github.com/Suvam-Bit/Road-Sign-Detection-TFOD/blob/main/sample_outputs/output_03.jpg?raw=true)
![alt text](https://github.com/Suvam-Bit/Road-Sign-Detection-TFOD/blob/main/sample_outputs/output_07.jpg?raw=true)
