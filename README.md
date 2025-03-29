# Object Detection using YOLOv8

## Overview
This project demonstrates object detection using YOLOv8 and OpenCV. It loads a pre-trained YOLOv8 model to detect objects in an image and display the results with bounding boxes and confidence scores.

## Features
- Uses YOLOv8 for object detection.
- Detects multiple objects in an image with high accuracy.
- Draws bounding boxes around detected objects.
- Displays object class names and confidence scores.
- Runs seamlessly on Google Colab and local environments.

## Installation
To run this project, install the required dependencies:

```bash
pip install opencv-python ultralytics
```

## Usage
1. **Load the YOLO model**: The script initializes YOLOv8 with a pre-trained model (`yolov8s.pt`).
2. **Input Image**: Provide an image file (e.g., `cat.jpeg`).
3. **Perform Object Detection**: The model processes the image and detects objects.
4. **Display Results**: The script overlays bounding boxes and labels on detected objects and displays the image.

## Running on Google Colab
If running on Google Colab, ensure you use `cv2_imshow()` to display images:

```python
from google.colab.patches import cv2_imshow
cv2_imshow(image)
```

For local execution, use:

```python
cv2.imshow('Object Detection', image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output
- The script prints detected object names and confidence scores.
- The image is displayed with bounding boxes and labels.

## Future Enhancements
- Extend the model to process videos in real-time.
- Improve accuracy by fine-tuning YOLO on a custom dataset.
- Deploy as a web application for easy accessibility.

## License
This project is licensed under the MIT License.

## Author
Developed by Kishore M

