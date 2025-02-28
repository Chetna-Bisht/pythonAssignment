# pythonAssignment
by Chetna Bisht

## Test Scene Feature Extraction

### Overview

This project involves extracting key features from a 2D image to analyze road infrastructure and billboards. The extracted information will provide insights into road structure, billboard placement, and potential distractions for drivers.
This project demonstrates object detection using the YOLO (You Only Look Once) model with OpenCV and NumPy.

### Dependencies

Ensure you have the required dependencies installed before running the notebook:

pip install opencv-python numpy matplotlib ultralytics

### Jupyter Notebook:

Open the Jupyter notebook

Run assignment.ipynb

Run each cell sequentially

### Problem Statement

From a given 2D image, the following features need to be extracted:

### Lane and Road Width Analysis

Detect the number of lanes on the road.

If lane markings are not visible, estimate the width of the road.

### Road Corner Detection

Identify and mark the corners of the road.

### Billboard Detection

Locate billboards in the image.

### Billboard Positioning

Determine whether the billboard is positioned on the Left-Hand Side (LHS), Right-Hand Side (RHS), or Overhead on the road.

### Billboard Size and Placement Analysis

Extract the following measurements for each billboard:

Width (W): The width of the billboard face.

Height (H): The height of the billboard face.

Elevation (E): The elevation of the billboard from the road level.

Setback Distance (D): The distance from the nearest billboard edge to the nearest road corner.

Angle (A): The orientation of the billboard face relative to the road.

### Occlusion Analysis

Detect and quantify the percentage of billboard face occluded by objects (e.g., buildings obstructing the view of the billboard).

### Billboard Clutter and Distraction Analysis

Identify billboards that are too close to each other, causing distraction or visual clutter.

Detect scenarios where a back billboard is overshadowed by a front billboard, reducing visibility and effectiveness.

### Billboard Distance Estimation

Measure the distance of the billboard from the image capture point.

If the image is taken with a zoom lens, calculate the relative distance of the billboard based on its apparent size in the zoomed image.

### Data Provided

The dataset includes reference sizes for billboards:

Width (W): The known width of the billboard.

Height (H): The known height of the billboard.

### Usage

Process the 2D image to detect and extract the above-listed features.

Utilize image processing techniques and computer vision algorithms to automate feature extraction.

Validate the extracted features against known reference data where applicable.

### Expected Output

Annotated image with detected features.

Numerical values representing extracted billboard dimensions, occlusion percentage, and positioning data.

Summary report highlighting the detected road and billboard attributes.
