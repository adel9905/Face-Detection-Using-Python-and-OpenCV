# Face Detection Using Python and OpenCV
## Overview
This project implements real-time face detection using Python and OpenCV. It leverages OpenCV’s Haar Cascade Classifier to detect faces from a webcam feed and marks detected faces with bounding rectangles on the video stream.


## Features
**Real-Time Face Detection**: Detects faces from a webcam feed with high accuracy.
**Easy-to-Use**: A simple script with minimal dependencies.
**Customizable**: Easily adjustable parameters for detection sensitivity and performance.


## Prerequisites

Ensure the following are installed on your system:
	1.	Python 3.6+: This project has been tested with Python 3.9.6.
	2.	OpenCV Library: The primary library used for image processing and face detection.

 ## Installation

**Step 1**: Clone the Repository.
bash
git clone <repository-url>
cd <repository-folder>

**Step 2**: Install Required Libraries
bash
python3 -m pip install opencv-python

## Usage
**Run the Script**:
Execute the following command to start the face detection program:
bash
python3 face_detection.py

	**Webcam Feed**:
The script will automatically access your system’s webcam. If the webcam feed does not appear, ensure your webcam is connected and enabled.

**Quit the Program**:
Press the q key at any time to exit the program.

## How It Works
	1.Pre-trained Model:
The script uses OpenCV’s pre-trained Haar Cascade Classifier for face detection. The model (haarcascade_frontalface_default.xml) is lightweight and efficient for real-time applications.
	2.	Face Detection:
	•	The script converts each webcam frame to grayscale.
	•	The Haar Cascade is applied to detect faces, returning bounding box coordinates for any detected faces.
	3.	Visualization:
Detected faces are highlighted with rectangles drawn over the video feed.

## Customization
	•	Detection Sensitivity:
Modify the scaleFactor and minNeighbors parameters in the script to adjust detection sensitivity and performance.
	•	Face Size:
Change the minSize parameter in the detectMultiScale method to filter out smaller or larger faces.

## Example Output

When the script is running, you will see a real-time webcam feed with blue rectangles around detected faces. Below is a snapshot example:

