# Digital Navigator: A Deep Learning-Based Virtual Mouse

## Project Overview

The **Digital Navigator** is an innovative virtual mouse system that provides a touchless and intuitive interface for controlling digital systems. This project leverages computer vision and deep learning techniques to offer a seamless alternative to traditional input devices like a mouse or keyboard. By translating specific hand gestures into standard mouse actions, it enhances accessibility and user experience for a wide range of applications, including smart home control and public interfaces.

## Features

The Digital Navigator system provides the following functionalities:

  * **Touchless Control:** Operates a virtual mouse entirely through natural hand gestures, eliminating the need for physical contact.
  * **Real-Time Processing:** Utilizes a standard webcam to continuously track and interpret hand movements in real time, ensuring immediate and responsive feedback.
  * **Comprehensive Gesture-Based Commands:** Translates specific hand poses into a variety of mouse actions:
      * **Mouse Movement:** The cursor accurately mimics hand movement when the index and middle fingers are extended.
      * **Left Click:** Performed by lowering the index finger while keeping the middle finger extended.
      * **Right Click:** Executed by extending the index finger and lowering the middle finger.
      * **Double Click:** Activated when both the index and middle fingers are brought together.
      * **Drag and Drop:** Enabled by closing the hand into a fist, allowing for seamless drag operations.
      * **No Action (Idle):** The system enters an idle state when all fingers are open, preventing accidental commands.
  * **Advanced Controls:** The system also includes advanced features for system control, such as:
      * **Volume Control:** Adjust system volume with a specific hand gesture.
      * **Brightness Control:** Change screen brightness using a designated gesture.
  * **Enhanced Accessibility:** Serves as a viable and effective alternative for users with mobility impairments or in environments where a physical mouse is impractical.

## Technologies and Libraries

This project is built using Python and relies on a suite of powerful libraries:

  * **`opencv-python` (OpenCV):** The primary computer vision library used for real-time video capture, frame processing, and drawing landmarks on the video feed.
  * **`mediapipe`:** A deep-learning framework from Google that provides robust solutions for detecting and tracking hand landmarks with high accuracy.
  * **`pyautogui`:** A cross-platform library that enables the script to programmatically control the mouse and keyboard, performing actions like movement, clicks, and scrolls.
  * **`pycaw`:** A Python wrapper for the Windows Core Audio APIs, used to control the system volume.
  * **`screen-brightness-control`:** A cross-platform library that allows the application to programmatically adjust screen brightness.
  * **`protobuf`:** Used internally by Mediapipe for data serialization and deserialization.
  * **`Pillow`:** A powerful image processing library used for handling images, particularly for the GUI.
  * **`tkinter`:** Python's standard GUI library, used to create the graphical user interface for the application.

## Software and Hardware Requirements

### Software

  * **Programming Language:** Python 3.x
  * **Integrated Development Environment (IDE):** Jupyter Notebook or IDLE Python 3.10 64-bit are recommended.

### Hardware

  * **Processor:** Intel Core i3, i5, i7 or higher
  * **RAM:** Minimum 8GB
  * **Storage:** 512GB SSD (1TB recommended)
  * **Peripherals:** A functional webcam is essential to capture hand movements.

## Installation and Setup

### 1\. Clone the Repository

You can clone the project from its GitHub repository:

```bash
git clone https://github.com/21AG1A05F0/Digital-Navigator.git
cd Digital-Navigator
```

### 2\. Install Dependencies

Before running the project, you need to install all the required libraries. Navigate to the project directory and run the following command to install them automatically:

```bash
pip install -r requirements.txt
```

### 3\. Run the Application

The system is designed to be run from an IDE or the command line.

  * To start the gesture controller, run the main Python script. The application will initialize the webcam and a GUI window.
  * Follow the on-screen instructions to begin controlling your mouse with hand gestures.

## How It Works

1.  **Webcam Initialization:** The program first initializes the webcam to capture a live video stream.
2.  **Hand Recognition:** Using MediaPipe, the system processes each video frame to detect and track the landmarks of your hand.
3.  **Gesture Classification:** The program analyzes the position of your fingers and hand landmarks to classify the current hand gesture.
4.  **Action Execution:** Based on the classified gesture, `pyautogui` executes the corresponding mouse or system action, such as moving the cursor, performing a click, or adjusting the volume.
5.  **Termination:** The program continues to run in real-time until you manually close the application window.
