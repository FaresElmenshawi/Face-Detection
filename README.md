# YOLOv4 Fine-Tuning for Face Detection

This repository contains code for fine-tuning the YOLOv4 object detection model for detecting faces in images and videos. The YOLOv4 model is pre-trained on the COCO dataset, which includes a "person" class but does not include a "face" class. In order to train the model to detect faces, we will fine-tune the pre-trained model on a dataset of annotated face images.


## Requirements
Python 3
OpenCV
Darknet (YOLOv4)

## Dataset
The dataset used for fine-tuning consists of images of faces along with annotations indicating the coordinates of the bounding boxes around each face..


## Fine-Tuning
To fine-tune the YOLOv4 model for face detection, follow these steps:

Prepare the dataset: Download the  dataset and convert it to the YOLOv4 format. 

Download the pre-trained weights: Download the pre-trained YOLOv4 weights from the official Darknet website.

Modify the YOLOv4 configuration file: Update the YOLOv4 configuration file yolov4.cfg to include a new class for faces. You can use the provided configuration file yolov4-obj.cfg as a template.

Train the model: Train the YOLOv4 model on the fine-tuning dataset using the darknet command-line tool. 

