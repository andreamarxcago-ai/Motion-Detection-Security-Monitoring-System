# Motion Detection Security Monitoring System (MDSMS)

## Project Description

The Motion Detection Security Monitoring System (MDSMS) is a computer vision project developed using Python and OpenCV. It detects motion by comparing consecutive camera frames and identifies moving regions using image processing techniques.

When motion is detected, the system displays a motion status, draws bounding boxes around detected areas, saves a snapshot, and records the security event in a CSV file. A dashboard provides an overview of the available security events and snapshots.

The current implementation is designed to run in Google Colab using browser-based webcam access.

## Features

* Webcam frame capture
* Grayscale image conversion
* Gaussian blur preprocessing
* Frame difference analysis
* Binary thresholding
* Contour detection
* Bounding box visualization
* Motion status display
* Security snapshot storage
* CSV event logging
* Security monitoring dashboard

## Setup Instructions

1. Open Google Colab at https://colab.research.google.com/.
2. Upload `Motion_Detection_Security_Monitoring_System.ipynb`.
3. Open the uploaded notebook.
4. Run the code cells in their intended order.
5. Allow webcam access when prompted.
6. Follow the notebook instructions to start motion detection.
7. Move an object in front of the camera to test motion detection.
8. Stop the live detection when finished.

## How the System Works

1. The system captures a webcam frame.
2. The frame is converted to grayscale.
3. Gaussian blur is applied to reduce small image variations.
4. Consecutive processed frames are compared using absolute frame difference.
5. Thresholding highlights pixels with sufficiently large changes.
6. Contours are extracted from the thresholded image.
7. Regions above the minimum contour area are marked with bounding boxes.
8. The system displays the motion status.
9. When a motion event begins, the system saves a snapshot and records the event in a CSV file.
10. The dashboard displays the available monitoring status, event history, and snapshots.
