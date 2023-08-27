##Object detection using SSD Mobile Net v3(2020_01_14) with large_coco

![Image of objects](/Road_Traffic.gif)

## Overview

This project demonstrates object detection using the Single Shot MultiBox Detector (SSD) model with MobileNet v3 as its base architecture. The model is pretrained on the COCO dataset, providing a strong foundation for real-time object detection tasks. This readme file provides instructions on how to set up and use this object detection system.

## Prerequisites

Before getting started, ensure you have the following:

- Python 3.6 or higher installed on your system.
- TensorFlow 2.x (2.2 or later) installed.
- OpenCV for image/video processing.
- GPU support is recommended for faster inference.

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/object-detection-ssd.git
    cd object-detection-ssd
    ```

2. Create a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use venv\Scripts\activate
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Download Pretrained Model**:

    Download the pretrained SSD MobileNet v3 (2020_01_14) with Large COCO model from the TensorFlow model zoo: [Download Link](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v3_large_coco_2020_01_14.tar.gz).

2. **Extract the Model**:

    Extract the downloaded model to the project directory.

3. **Inference**:

    - Modify the `detect_objects.py` script to specify the path to the image or video you want to process.
    - Run the detection script:

        ```bash
        python objectdetection_v3.py
        ```

    The detected objects will be outlined with bounding boxes, and the results will be displayed on the screen or saved to an output file, depending on your configuration.

## Customization

You can customize this object detection system by:

- Fine-tuning the model on your specific dataset for improved accuracy on custom object categories.
- Adjusting confidence thresholds and non-maximum suppression parameters in the `detect_objects.py` script to control the detection sensitivity.
- Implementing real-time object detection in applications, such as surveillance systems or robotics.


## Acknowledgments

- [TensorFlow Model Zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md) for pretrained models.
- [OpenCV](https://opencv.org/) for image and video processing.
- The TensorFlow and OpenCV communities for their valuable contributions and resources.
