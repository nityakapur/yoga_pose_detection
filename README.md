# Yoga Pose Detection Through EfficientNetB0 and ResNet50
## Objective

The project focuses on drawing clear comparison between EfficientNetB0 and ResNet50 by training the models for Human Pose Estimation Task. The models are trained on 3 datasets which are built from scratch. The datasets defer with respect to number of classes (107 and 54) as well as image preprocessing steps such as data augmentation, contour generation and mediapipe joints plotting.

## Image Preprocessing Steps

### Mirror Images
To augment the dataset, all images were mirrored horizontally using Python’s OpenCV library. This step doubles the dataset size, ensuring the model is exposed to pose variations and increasing generalizability.

![image](https://github.com/user-attachments/assets/85499ca4-b0d3-4cf9-b28e-55be03aea29d)

### Contours
Contours were added to approximately 6 images per class to enhance structural integrity and emphasize pose outlines. This preprocessing step uses edge detection techniques to highlight critical posture features, improving the model’s ability to classify poses accurately.

![image](https://github.com/user-attachments/assets/600d5e7a-b829-42ca-a406-0c5f1946edee)

### Mediapipe
 The human pose joints are also taken into consideration during the lateral part of study. This has been done by application of a media pipe to calculate joints and generate images in the dataset. This helped in increasing images in the dataset and betterment of overall accuracy.

![image](https://github.com/user-attachments/assets/d8ea5aed-b089-4d6f-83ba-dd1eb931f5f4)

## Best Fit Dataset

Best fit dataset is created from scratch - consists of 10,369 images with preprocessed images using contours, mediapipe and data augmentation. It helped in classifying 54 Yoga Poses and can give accuracte results on images and good results for videos. The break down for the same can be seen below:

![image](https://github.com/user-attachments/assets/2c2c17a7-f99c-4730-a09a-1688f75db203)


## Results 

EfficientNetB0 helps in obtaining the best accuracy of 88.34% and loss of 0.5114. EfficientNetB0 was also tried and tested for this project due to a further usecase of deploying current model into a Mobile Application. This would help in creating a mobile health companion which can further input raw images from user and detect poses in real time, as to guide users and help them inculcate yoga in their everyday life. The resultant table for the same can be seen below :

![image](https://github.com/user-attachments/assets/fde11cf9-5a61-4272-9f6b-75dd20fccb3e)


 
