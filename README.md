
### Lane Detection using OpenCV
This repository contains a Python-based computer vision application that detects and highlights lane lines in a video. The script processes a video frame-by-frame, applying a series of image processing techniques to identify the road's lane markings.

### Key Features
Image Processing Pipeline: Converts video frames to grayscale, applies a Gaussian blur, and uses Canny edge detection to find edges.

Region of Interest (ROI): Masks a specific triangular area of the frame to focus the detection on the road ahead.

Hough Transform: Utilizes the Probabilistic Hough Transform to detect straight lines from the processed image.

Lane Averaging: Averages the detected line segments to create a single, stable representation for both left and right lanes.

Output Visualization: Overlays the detected lane lines onto the original video frame for a clear visual output.

### Technologies Used
Python: The core programming language for the script.

OpenCV (cv2): Used for video processing, image manipulation, and visual output.

NumPy (numpy): Utilized for efficient numerical operations and array manipulation.

### How to Run
Prerequisites: Ensure you have Python, OpenCV, and NumPy installed. You can install the required libraries with pip:

              pip install opencv-python numpy

Video File: Update the video file path in the code to point to your local video file. The current path is:

             cap = cv2.VideoCapture("C:/Users/HP/Downloads/test1.mp4")

             Replace "C:/Users/HP/Downloads/test1.mp4" with the correct path to your video.

Execution: Run the Python script from your terminal:

            python your_script_name.py


