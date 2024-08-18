Real-Time Yawn Detection Using OpenCV and Dlib
This project implements a real-time yawn detection system using OpenCV and Dlib. The system captures video from a webcam, detects faces, and analyzes the facial landmarks to determine if a person is yawning. If a yawn is detected, an alert message is displayed on the video feed.

Features
Real-Time Detection: Detects yawning in real-time using a webcam feed.
Facial Landmark Detection: Utilizes Dlib’s pre-trained model to detect 68 facial landmarks.
Yawn Detection: Computes the mouth aspect ratio (MAR) to determine if the mouth is open wide enough to be classified as a yawn.
Visual Feedback: Displays a message on the video feed when a yawn is detected.
Requirements
Python 3.x
OpenCV 4.x (opencv-python package)
Dlib (dlib package)
Numpy (numpy package)
Installation
To set up this project, follow these steps:

Install Required Python Packages:

Install the necessary Python packages using pip:

bash
Copy code
pip install opencv-python dlib numpy
Download Facial Landmark Predictor:

Download the shape_predictor_68_face_landmarks.dat file from dlib's model zoo and place it in the Yawn Detector/ directory.

Usage
Run the Yawn Detection System:

Execute the Python script to start the real-time yawn detection:

bash
Copy code
python yawn_detector.py
Quit the Application:

Press q on the keyboard to exit the application and close the video feed.

How It Works
Video Capture: Captures video from the default webcam.
Face Detection: Detects faces in the video stream using Dlib's frontal face detector.
Landmark Detection: Detects 68 facial landmarks on the detected faces.
Mouth Aspect Ratio (MAR): Calculates the mouth aspect ratio to monitor the degree of mouth opening.
Yawn Detection: If the mouth aspect ratio is below a certain threshold, a yawn is detected, and a message is displayed.
Display Results: The video feed with detected yawns is displayed in real-time.
File Descriptions
yawn_detector.py: The main Python script that runs the real-time yawn detection using OpenCV and Dlib.
shape_predictor_68_face_landmarks.dat: Pre-trained model file used for detecting facial landmarks. (Download separately from Dlib’s website).
Contributing
Contributions to improve the project are welcome. Please fork the repository and submit a pull request with your changes.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

