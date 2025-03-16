# Object Detection Using OpenCV and HSV Masking

## Description
This project uses OpenCV and HSV color filtering to detect a specific color (yellow) in a video stream from a webcam. It highlights the detected object by drawing a bounding box around it.

## Features
- Captures video feed from the webcam
- Converts the frame to HSV color space
- Creates a mask to detect objects of a specified color
- Draws a bounding box around the detected object
- Displays the processed video feed in real-time

## Prerequisites
Ensure you have the following installed before running the project:
- Python 3.x
- OpenCV (`cv2`)
- NumPy (`numpy`)
- PIL (`Pillow`)

## Installation
1. Clone or download this repository.
2. Install the required dependencies using pip:
   ```bash
   pip install opencv-python numpy pillow
   ```

## Usage
1. Run the main script:
   ```bash
   python main.py
   ```
2. The script will open a webcam feed and detect objects of the specified color.
3. Press `q` to exit the program.

## Project Structure
```
project-folder/
│── main.py       # Main script for color detection
│── util.py       # Utility script containing helper functions
```

## Code Overview

### `main.py`
- Captures video from the webcam.
- Converts frames to HSV color space.
- Applies a color mask to detect objects.
- Draws a bounding box around detected objects.
- Displays the processed video in real-time.

### `util.py`
- Defines the `get_limits(color)` function to calculate HSV limits for a given RGB color.
- Helps in creating an HSV mask for object detection.

## Customization
- To detect a different color, change the `yellow` variable in `main.py` to the desired RGB value:
  ```python
  yellow = [0, 255, 255]  # Change this to your target color
  ```





