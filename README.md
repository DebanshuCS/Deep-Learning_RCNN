# Deep-Learning_RCNN

## Problem statement:

Due to the varied backgrounds in the pictures and variations in data gathering conditions brought on by the sensor geometry and atmospheric factors, detecting aeroplanes from satellite photography is a difficult operation. For the automated identification of aeroplanes, deep learning techniques offer dependable and accurate solutions; nevertheless, a sizable amount of training data is needed to get promising results.

## About the project:

In this project, I used photos from Google Earth (GE) and identify the bounding box of each plane to generate an unique aeroplane identification dataset called High Resolution Planes (HRPlanes). To reflect a diversity of landscape, seasonal, and satellite geometry circumstances acquired from various satellites, HRPlanes includes GE photos of several airports all around the world.

We tested our dataset using two popular object detection algorithms, YOLOv7 and Faster R-CNN. My first finding indicate that the used dataset has the potential to be an important data source and benchmark data set for future applications. Furthermore, the proposed architecture and findings of this work might be applied to transfer learning of other datasets and models for aeroplane detection.

## Exaplanation:

To address the object detection problem using deep learning was the R-CNN (Regions with CNN features) model.This model used a combination of region proposal algorithms and convolutional neural networks (CNNs) to detect and localize objects in images.

![63c69544f9b0972c0606d735_One and two stage detectors object detection-min](https://user-images.githubusercontent.com/118846871/218386709-8b63d888-2819-4c49-a8a2-874cc714c8e1.jpg)

YOLO is a single-shot detector that uses a fully convolutional neural network (CNN) to process an image.

Overall, the choice between single-shot and two-shot object detection depends on the specific requirements and constraints of the application.


### YoloV7 Detection: 

![yolo](https://user-images.githubusercontent.com/118846871/218386202-748310ac-ed75-47ec-ade3-da5faa5229ca.png)
![download](https://user-images.githubusercontent.com/118846871/218386241-07be5ede-d9c1-4fa1-a027-425958f90771.png)

Intersection over Union is a popular metric to measure localization accuracy and calculate localization errors in object detection models.

To calculate the IoU between the predicted and the ground truth bounding boxes, we first take the intersecting area between the two corresponding bounding boxes for the same object. 
Following this, we calculate the total area covered by the two bounding boxes— also known as the “Union” and the area of overlap between them called the “Intersection.”

The intersection divided by the Union gives us the ratio of the overlap to the total area, providing a good estimate of how close the prediction bounding box is to the original bounding box.

![yolo1](https://user-images.githubusercontent.com/118846871/218385836-d08cff2d-fce1-4eec-8ca2-40a69b6adfcb.png)
