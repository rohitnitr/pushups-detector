
# Push-Up Detector

This project is a push-up detector that uses computer vision techniques to identify and count push-up exercises performed by a person in front of a camera.

## Prerequisites

Before running the push-up detector, make sure you have the following dependencies installed:

- Python 3.7 or higher
- OpenCV (cv2)
- Mediapipe
- NumPy

You can install the required dependencies using the following command:

```bash
pip install opencv-python mediapipe numpy
```

## Usage

To use the push-up detector, follow these steps:

1. Clone the repository:

```bash
https://github.com/rohitnitr/pushups-detector.git
```

2. Change into the project directory:

```bash
cd push-up-detector
```

3. Run the `detect_pushups.py` script:

```bash
python detect_pushups.py
```

4. Follow the prompts displayed on the screen. Type 'yes' to start the push-up detection.

5. A video window will open showing the camera feed with push-up detection results. The program will track your body movements and display whether you are performing a push-up or not.

6. To exit the program, press 'q' on your keyboard. If you want to close the operation before that, press 'x' and type 'yes' when prompted.

## How It Works

The push-up detector uses the OpenCV library and the Mediapipe framework to detect the person's body landmarks and track their movements. It specifically focuses on the positions of the left shoulder, right shoulder, and left hip to calculate the angle formed during a push-up exercise. If the angle exceeds a certain threshold (160 degrees in this case), it classifies it as a push-up.

The program continuously processes frames from the camera and updates the push-up count whenever a valid push-up is detected. If no push-ups are detected for a certain number of consecutive frames, it displays a message indicating that push-ups couldn't be detected.


