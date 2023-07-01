# opencv-face-recognition


The Face Recognition App is a Python application that utilizes computer vision techniques to detect and recognize faces in real-time. It provides functionality for capturing faces, training a recognition model, and performing face recognition on live video streams.

## Features

- Capture faces using the webcam.
- Train a face recognition model based on the captured images.
- Perform real-time face recognition on live video streams.
- Display recognized faces with labels in the video feed.

## Prerequisites

Before running the Face Recognition App, make sure you have the following prerequisites installed:

- Python 3.6 or later
- OpenCV library
- NumPy library

## Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/sid209e/opencv-face-recognition.git
```

2. Navigate to the project directory:

```bash
cd opencv-face-recognition
```


3. Install the required dependencies:

```bash
pip install -r requirements.txt
```


## Usage

### 1. Capture Faces

The `capture_faces.py` script allows you to capture faces using the webcam. It prompts you to enter a person's name, captures their face images, and saves them in the `dataset` folder.

To capture faces, run the following command:

```bash
python capture_faces.py
```

Follow the on-screen instructions to provide person names and save the captured images.

### 2. Train Faces

The `train_faces.py` script trains a face recognition model based on the captured images in the `dataset` folder. It utilizes the OpenCV library and the LBPH (Local Binary Patterns Histograms) algorithm for training.

To train the face recognition model, run the following command:

```bash
python train_faces.py
```


The trained model will be saved in the `recognizer` folder as `encodings.pickle`.

### 3. Perform Face Recognition

The `face_recognition.py` script performs real-time face recognition on live video streams from the webcam. It utilizes the trained face recognition model to recognize faces and displays recognized faces with labels in the video feed.

To perform face recognition, run the following command:

```bash
python face_recognition.py
```


The script will load the trained model from the `recognizer` folder and start the face recognition process. Recognized faces will be displayed with labels in the video feed.

Press `q` to exit the face recognition application.

## Dataset and Model

- The captured face images are stored in the `dataset` folder. Each person's face images are saved in separate subfolders with their respective names.
- The trained face recognition model is saved as `encodings.pickle` in the `recognizer` folder. This model is used for face recognition in the `face_recognition.py` script.

## License

This project is licensed under the GNU General Public License (GPL). See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions to the Face Recognition App are welcome! If you have any ideas, improvements, or bug fixes, please open an issue or a pull request.

## Acknowledgments

This project was inspired by the work of various computer vision and face recognition libraries and tutorials. I would like to acknowledge their contributions.

