# Pose-Estimation-using-MediaPipe

# Human Activity Recognition using Pose Estimation
**Course:** Computer Vision ( Complex Computing Problem )  
**Student:** Sabiha Pirzadah | 23-AI-84  
**Instructor:** Engr Hamza Farooqui  



## What This Project Does
This notebook detects human poses in a video, computes joint angles, 
and classifies activities (Arm Down / Arm Raised) using a rule-based system.


## How It Works
1. MediaPipe extracts 33 body keypoints from each video frame
2. Keypoint coordinates are smoothed using a Savitzky-Golay filter
3. Angles are computed at the Right Shoulder, Right Elbow, and Right Wrist
4. A simple rule classifies each frame based on the shoulder angle



## Libraries Required
- mediapipe
- opencv-python
- numpy
- matplotlib
- scipy

Install all with:
pip install mediapipe opencv-python numpy matplotlib scipy



## Video Used
Personal recording  WIN_20260523_14_01_59_Pro.mp4  
Two activities performed: Arm Down and Arm Raised



## Results
- Total frames: 313
- Transition frames: 169, 292
- Classification accuracy: 100%
