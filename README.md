# Face_Recognition_Project
Project Code: https://drive.google.com/drive/folders/13ONn9GRcRtTX5ct0QNrYkTFmIG9kAE55?usp=sharing
## Description

This project develops a face recognition system integrated into a **WeChat Mini-Program**, with a **Flask** backend to handle server-side operations. The system encompasses three primary functions: face detection, face recognition, and face landmark detection. Each function is trained using **TensorFlow**, leveraging datasets such as WIDER FACE, FaceV5, and 300W_LP to ensure high accuracy and performance.

## Functions

### Face Detection:
<div align="center">
  <img src="https://github.com/FakeJackJia/Face_Recognition_Project/blob/main/Example/Face%20Detection.gif" width="300" height="400" />
</div>

- **Overview**: Real-time face detection and framing faces.
- **Dataset Used**: WIDER FACE
- **Model**: SSD Model embedded in TensorFlow (Code modified to fit this task).

### Face Recognition
<div align="center">
  <img src="https://github.com/FakeJackJia/Face_Recognition_Project/blob/main/Example/Face%20Recognition.gif" width="300" height="400" />
</div>

- **Overview**: First, a face is registered into the database; then, you may log in if the system correctly identifies your face.
- **Dataset Used**: FaceV5
- **Model**: FaceNet (https://github.com/davidsandberg/facenet)

### Face Landmark
<div align="center">
  <img src="https://github.com/FakeJackJia/Face_Recognition_Project/blob/main/Example/Face%20Landmark.gif" width="300" height="400" />
</div>

- **Overview**: Real-time showing 68 key points of faces.
- **Dataset Used**: 300W_LP
- **Model**: SENet (Built from scratch)

## Note
- Tensorflow 1.14 is used to train the model
- All datasets are preprocessed and saved in the TFRecord file
- All models are saved in pb file
- Flask is used to perform backend operations
