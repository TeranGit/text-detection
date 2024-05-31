# Python OpenCV Text Detection

A demo application for text detection using Python, OpenCV, and TensorFlow.

## Description

This project demonstrates text detection in images and video streams using the EAST text detector model with OpenCV and TensorFlow. It includes scripts for detecting text in both static images and live video streams from a camera.
![](https://github.com/TeranGit/text-detection/blob/main/demo.png)
## Installation

### Prerequisites

- [Python](https://www.python.org/downloads/) 3.6 or higher
- [pip](https://pip.pypa.io/en/stable/installation/)

### Installing Dependencies

Run the following command to install the required Python packages:

```bash
pip install numpy opencv-python imutils

Usage
Text Detection in Images
To detect text in an image, use the following command:
python text_detection.py --image images/lebron_james.jpg --east frozen_east_text_detection.pb

This command will start the video stream using your camera, and any text in the frame will be detected and highlighted.

Arguments
--east : Path to the input EAST text detector model.
--image : Path to the input image file (for image text detection).
--video : Path to the optional input video file (for video text detection).
--min-confidence : Minimum probability required to inspect a region (default: 0.5).
--width : Resized image width (should be multiple of 32, default: 320).
--height : Resized image height (should be multiple of 32, default: 320).

Example Commands
Image Text Detection
python text_detection.py --image images/sample.jpg --east frozen_east_text_detection.pb --min-confidence 0.5 --width 320 --height 320

Video Text Detection
python main.py --east frozen_east_text_detection.pb --min-confidence 0.5 --width 320 --height 320

Contributing
Fork the repository.
Create your feature branch (git checkout -b feature/AmazingFeature).
Commit your changes (git commit -m 'Add some AmazingFeature').
Push to the branch (git push origin feature/AmazingFeature).
Open a Pull Request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
OpenCV
TensorFlow
EAST: An Efficient and Accurate Scene Text Detector
