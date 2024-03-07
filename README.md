# Hand Gesture Presentation Controller👋🖥️

## Overview

This Python script utilizes the `cvzone.HandTrackingModule` and `cv2` libraries to create a presentation controller based on hand gestures. The code captures webcam input, detects hand gestures, and allows the user to control a presentation using specific gestures.

## Features

- **Gesture Controls:**
  - Swipe left (gesture-1) to move to the previous slide.
  - Swipe right (gesture-2) to move to the next slide.
  - Display a pointer (gesture-3) using two fingers.
  - Drawing mode (gesture-4) with a single finger, allowing annotations on the slides.
  - Erase annotations (gesture-5) using three fingers.

- **Presentation Images:**
  - The code assumes presentation images are stored in the "Presentation" folder.
  - Images are loaded in sorted order for sequential navigation.

## Prerequisites

- Python 3.x
- OpenCV (`cv2`)
- `cvzone` library

## Installation

1. Install required libraries:

   ```bash
   pip install opencv-python
   pip install cvzone
   ```

2. Run the script:

   ```bash
   python presentation_controller.py
   ```

## Usage

1. Ensure the webcam is connected and functioning.
2. Execute the script and open the presentation.
3. Use specified hand gestures to control the presentation as described in the "Features" section.

## Gesture Descriptions

- **Swipe Left (gesture-1):**
  - Move to the previous slide.

- **Swipe Right (gesture-2):**
  - Move to the next slide.

- **Pointer Display (gesture-3):**
  - Display a red circle as a pointer using two fingers.

- **Drawing Mode (gesture-4):**
  - Enable drawing mode with a single finger.
  - Annotations are drawn on the current slide.

- **Erase Annotations (gesture-5):**
  - Erase the last annotation using three fingers.

## Configuration

- **Parameters:**
  - `width`, `height`: Width and height of the camera feed.
  - `gestureThreshold`: Threshold for detecting hand gestures.
  - `folderPath`: Path to the folder containing presentation images.
  - `detectionCon`: Confidence threshold for hand detection.
  - `maxHands`: Maximum number of hands to detect.

## Acknowledgments

- This script utilizes the `cvzone` library for hand tracking.
