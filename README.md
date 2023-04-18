# Realtime Face Mask Detection with YOLOv4

This repository contains code for real-time face mask detection using the YOLOv4 object detection model. The YOLOv4 model is fine-tuned on a dataset of annotated images of people wearing and not wearing masks. The model can detect faces as well as classify whether the person is wearing a mask or not.

## Requirements
Python 3
OpenCV
Darknet (YOLOv4)

## Dataset
The dataset used for fine-tuning consists of images of people wearing and not wearing masks, along with annotations indicating the coordinates of the bounding boxes around each face and whether the person is wearing a mask or not.

## Fine-Tuning
To fine-tune the YOLOv4 model for real-time face mask detection, follow these steps:

Prepare the dataset: Download the dataset and convert it to the YOLOv4 format.

Download the pre-trained weights: Download the pre-trained YOLOv4 weights from the official Darknet website.

Modify the YOLOv4 configuration file: Update the YOLOv4 configuration file yolov4.cfg to include new classes for "with_mask" and "without_mask". You can use the provided configuration file yolov4-custom.cfg as a template.

Train the model: Train the YOLOv4 model on the fine-tuning dataset using the darknet command-line tool.

Test the model: Test the model on images and videos to verify its performance in real-time face mask detection.

Note: The model may need to be re-trained periodically as new face mask styles emerge.

