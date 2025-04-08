# Sign-Language-Classification-Detection
This project implements a real-time sign language recognition system using computer vision and deep learning. Leveraging OpenCV, MediaPipe-based hand tracking (via CVZone), and a custom-trained Convolutional Neural Network (CNN) model, the system can accurately classify hand gestures representing common sign language phrases.
The system is designed in two key components:

Sign Language Data Collection Script
A dynamic hand gesture capturing pipeline that detects a single hand in real time, crops and preprocesses the region of interest (ROI) with aspect-ratio preservation, and saves standardized 300×300 images to a dataset directory for training. This script enables efficient and consistent data gathering across multiple gesture classes.

Gesture Recognition and Classification Pipeline
The main classification script detects and isolates the user's hand from webcam input, preprocesses the ROI using padding and resizing while maintaining spatial consistency, and passes the processed image into a pre-trained Keras model for gesture classification. The output label is then overlaid on the live video feed along with bounding boxes for visual feedback.

Created by Shubham Pandey
