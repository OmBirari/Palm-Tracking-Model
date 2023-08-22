# Palm-Tracking-Model
![Img](https://github.com/OmBirari/Palm-Tracking-Model/assets/111376587/52ccecdc-4de8-477f-9c13-a9c300566a27)
<br> # Hand Detection and Tracking using OpenCV and MediaPipe

This repository contains a Python script that demonstrates hand detection and tracking using the OpenCV library and the MediaPipe framework. The script utilizes the MediaPipe Hands module to detect and track hand landmarks in real-time using your computer's webcam.

## Requirements

Before running the script, make sure you have the following libraries installed:

- OpenCV
- MediaPipe

You can install these libraries using the following commands:

pip install opencv-python
pip install mediapipe


## How to Use

1. Clone this repository to your local machine.
   git clone https://github.com/OmBirari/hand-detection.git

2. Navigate to the repository directory.
   cd hand-detection

3. Run the script.
   python hand_detection.py
   
4. A window will pop up showing the webcam feed with hand landmarks drawn on the detected hands. Press the 'z' key to exit the application.

## Script Overview

The `hand_detection.py` script demonstrates hand detection and tracking using the `handDetector` class. This class encapsulates the functionality of detecting hands and extracting their landmarks using MediaPipe. The script initializes the class, captures webcam frames, processes the frames to find and draw hand landmarks, and calculates frames per second (FPS) information.

## Class `handDetector`

This class provides methods to detect and track hands using MediaPipe's Hands module. It includes the following methods:

- `__init__(self, mode=False, maxHands=2, detectionCon=0.5, trackCon=0.5)`: Constructor to initialize the hand detection parameters.

- `findHands(self, img, draw=True)`: Detects hands in the given image and optionally draws landmarks and connections.

- `findPosition(self, img, handNo=0, draw=True)`: Extracts the landmarks of a specific hand and optionally draws points on the image.

## Acknowledgments

This code is based on tutorials and examples from OpenCV and MediaPipe. Feel free to modify and extend this code for your projects.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.




