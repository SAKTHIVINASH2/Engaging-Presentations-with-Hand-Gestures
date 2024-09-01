# Engaging-Presentations-with-Hand-Gestures

## Introduction:
This project aims to create an interactive presentation tool that uses hand gestures to control various actions. By recognizing the number of fingers a user is holding up, the application will perform corresponding operations, such as moving forward, moving backward, pointing, writing, and undoing writing.

## To install the 3D Motion Capture From Video, please follow these steps:
1. Clone the repository to your local machine.
2. Install the required dependencies by running the following command:

```
pip install -r requirement.txt
```


## Libraries used:
* OpenCV (cv2): For image processing and computer vision tasks.
* MediaPipe: A framework for building ML-powered pipelines for a variety of tasks, including hand tracking.
* HandDetector: It is a powerful tool within the OpenCV (cv2) library that enables real-time hand detection and tracking. It leverages advanced computer vision techniques to accurately locate and identify human hands in video or image data.

## Workflow:

1. Initialize Libraries and Variables:
   * Import necessary libraries.
   * Set up video capture and initialize MediaPipe's hand detection model.
   * Define variables for hand landmarks, finger counts, and action states.
     
2. Capture Video and Detect Hands:
   * Continuously capture video frames from a webcam.
   * Process each frame using MediaPipe's hand detection model to locate and track hands.

3. Extract Hand Landmarks:
   * Extract the key points (landmarks) of the detected hands.

4. Determine Finger Count:
   * Use the landmark positions to calculate the number of fingers being held up.
   * Implement logic to recognize specific hand gestures (e.g., pointing, writing).

5. Perform Actions Based on Finger Count:
   * Based on the recognized finger count and position, trigger corresponding actions:
     1. Five finger: Move forward.
     2. Four fingers: Move backward.
     3. Two fingers: Point.
     4. One fingers: Write.
     5. Three fingers: Undo writing.
   * Image representation:
     
     <img src="Document/finger count and position for specific operation.jpg" width="60%"/>

6. Visualize Hand Detection and Actions:
   * Overlay the detected hand landmarks and action indicators on the video frames.
   * Display the processed video in a window.
