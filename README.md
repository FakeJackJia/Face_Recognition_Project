# Face_Recognition_Project

## Description

This project develops a face recognition system integrated into a **WeChat Mini-Program**, with a **Flask** backend to handle server-side operations. The system encompasses three primary functions: face detection, face recognition, and face landmark detection. Each function is trained using **TensorFlow**, leveraging datasets such as WIDER FACE, FaceV5, and 300W_LP to ensure high accuracy and performance.

## Functions

### Face Detection: 

- **Overview**: Real-time face detection and framing faces.
- **Dataset Used**: WIDER FACE
- **Model**: SSD Model embedded in TensorFlow (Code modified to fit this task).

### Face Recognition

- **Overview**: First, a face is registered into the database; then, you may log in if the system correctly identifies your face.
- **Dataset Used**: FaceV5
- **Model**: FaceNet (https://github.com/davidsandberg/facenet)

### Face Attribute

- **Overview**: Real-time showing 68 attribute points of faces.
- **Dataset Used**: 300W_LP
- **Model**: SENet (Built from scratch)

# Note
- Tensorflow 1.14 is used
- Flask is used to perform backend operations
- WeChat Mini-Program is built using JS and CSS
