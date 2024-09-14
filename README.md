# BodyPostureDetection
# Real-Time Posture Detection Using Mediapipe and OpenCV

This project implements a real-time posture detection system using Mediapipe and OpenCV in Python. The system analyzes key points from a video stream (such as from a webcam) and computes angles of neck and torso inclination to monitor posture. If poor posture is detected for over 30 seconds, an alert is displayed.

## Features
- Real-time detection of body landmarks using Mediapipe
- Calculation of neck and torso inclination angles
- Real-time alert system for poor posture
- Video recording of the posture analysis output


## How It Works
The code captures video frames, identifies key body landmarks (shoulders, ear, hips), and calculates angles that help detect poor posture. A warning is displayed if the person maintains bad posture for more than 30 seconds.

1. **Key Libraries Used:**
    - `Mediapipe`: For detecting body landmarks.
    - `OpenCV`: For video capture and frame processing.
    - `Math`: For calculating distances and angles.

2. **Posture Evaluation:**
    - **Neck Inclination**: The angle between the left shoulder and left ear.
    - **Torso Inclination**: The angle between the left hip and left shoulder.
    - **Alert Condition**: When neck inclination is less than 40 degrees and torso inclination is less than 10 degrees, posture is considered bad.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/urboitaeef/BodyPostureDetection.git
   cd posture-detection
