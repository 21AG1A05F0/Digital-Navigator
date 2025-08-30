# Digital Navigator using Deep Learning

A hand gesture recognition-based virtual mouse system that provides an intuitive and touchless interface for controlling digital systems. This project leverages computer vision and deep learning techniques to offer an alternative to traditional input devices like a mouse or keyboard, improving accessibility and user experience.

## Features

The Digital Navigator system provides the following functionalities:

  * **Touchless Control:** Operates a virtual mouse using only hand gestures.
  * **Real-Time Processing:** Continuously tracks hand movements using a webcam for immediate feedback.
  * **Gesture-Based Commands:** Translates specific hand gestures into standard mouse actions.
      * **Mouse Movement:** Cursor moves when the index and middle fingers are up.
      * **Left Click:** Performed when the index finger is down and the middle finger is up.
      * **Right Click:** Executed when the index finger is up and the middle finger is down.
      * **Double Click:** Activated when both the index and middle fingers are together.
      * **Drag and Drop:** Enabled by closing the hand into a fist.
      * **No Action (Idle):** The system is in an idle state when all fingers are open.
  * **Alternative Input:** Serves as a viable alternative for users with mobility impairments or for applications like smart home control and public interfaces.

## Technologies Used

  * **Programming Language:** Python
  * **Libraries:**
      * `cv2` (OpenCV): A computer vision library used for real-time video capture and frame processing.
      * `mediapipe`: A deep-learning framework for detecting and tracking hand landmarks.
      * `pyautogui`: Employed to perform mouse actions based on recognized gestures.
      * `math`: A standard Python library for mathematical operations.
      * `pycaw`: Python Core Audio Windows Library.
      * `screen-brightness-control`: A cross-platform library for controlling screen brightness.
      * `protobuf`: A library used by Mediapipe.
      * `Pillow`: A library used for image manipulation.
  * **Models:** Deep Learning Computer Vision Models.

## Software and Hardware Requirements

  * **Software:**
      * **IDE:** Jupyter Notebook, IDLE Python 3.10 64-bit.
  * **Hardware:**
      * **Processor:** Intel Core i3, i5, i7 or higher.
      * **RAM:** Minimum 8GB.
      * **Storage:** 512GB SSD (1TB recommended).
      * **Peripherals:** A webcam is required to capture hand movements.

## Installation and Setup

### 1\. Install Required Packages

First, ensure you have Python and `pip` installed. Then, run the following command to install all the necessary libraries:

```bash
pip install opencv-python mediapipe pyautogui pycaw screen-brightness-control protobuf Pillow
```

### 2\. Run the Project

The system is designed to be run from an IDE like Jupyter Notebook or IDLE.

1.  **Start Webcam Capture:** The program initializes the webcam to capture video frames in real time.
2.  **Hand Recognition:** The system uses MediaPipe and OpenCV to detect and track hand landmarks.
3.  **Gesture Processing:** The system classifies gestures based on finger positions.
4.  **Action Execution:** Recognized gestures are mapped to specific mouse actions (e.g., movement, clicks, drag and drop).

The program will continue running until you manually terminate it.
