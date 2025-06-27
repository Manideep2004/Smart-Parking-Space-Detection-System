# Smart-Parking-Space-Detection-System
Parking Space Detection System
A computer vision-based parking space detection system that can identify and monitor available parking spaces in real-time using OpenCV and Python.
Features

Interactive Parking Space Setup: Click-and-drag interface to define parking spaces
Real-time Detection: Automatically detects occupied and free parking spaces
Visual Feedback: Color-coded rectangles (green for free, red for occupied)
Space Counter: Displays the number of available spaces
Video Processing: Works with video files for continuous monitoring

Prerequisites
Before running the system, make sure you have the following installed:
bashpip install opencv-python
pip install cvzone
pip install numpy
Files Description
1. ParkingSpacePicker.py
Interactive tool for defining parking spaces on your parking lot image.
Features:

Left-click to add a parking space
Right-click to remove a parking space
Automatically saves parking positions to CarParkPos file

2. main.py
Main detection system that processes video feed and identifies parking space occupancy.
Features:

Loads predefined parking positions
Processes video frames with image filtering
Detects space occupancy using pixel counting
Displays real-time results with visual indicators

Setup Instructions
Step 1: Prepare Your Files

Place your parking lot image as carParkImg.png in the project directory
Place your parking lot video as carPark.mp4 in the project directory

Step 2: Define Parking Spaces

Run the parking space picker:
bashpython ParkingSpacePicker.py

Click on each parking space in your image to define them
Use right-click to remove incorrectly placed spaces
Close the window when done (positions are automatically saved)

Step 3: Run Detection System

Start the main detection system:
bashpython main.py

The system will display the video with:

Green rectangles for free spaces
Red rectangles for occupied spaces
Pixel count for each space
Total available spaces counter
