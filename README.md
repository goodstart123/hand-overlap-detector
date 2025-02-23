# Hand Intersection Detection System

## Methods and Libraries Used

This system utilizes the **MediaPipe Hands** library for hand detection and tracking within a video. The **OpenCV** library is employed for video processing, and the **Intersection over Union (IoU)** algorithm is used to detect hand intersections.

## System Description

The system operates as follows:

1. A video is uploaded and processed using **OpenCV**.
2. In each frame, the **MediaPipe Hands** library detects and tracks hands.
3. Hand positions are used as input for the **IoU** algorithm, which determines if the hands are intersecting.
4. If hands are intersecting, an alert is displayed on the frame, and the frame border flashes.
5. The processed video is saved.

## Challenges and Solutions

* **Challenge:** Hand detection accuracy was insufficient.
* **Solution:** Parameters of the **MediaPipe Hands** library were adjusted to enhance detection accuracy.

* **Challenge:** Hand intersection detection was not reliable enough.
* **Solution:** The threshold of the **IoU** algorithm was modified to improve the reliability of intersection detection.

## System Startup Instructions

1. Install the necessary libraries: `pip install opencv-python mediapipe`.
2. Upload your video to the Colab environment.
3. Run the code.
4. The processed video will be saved in the Colab environment.
