# ASL_Recognition-Project
Here is a `README.md` file for your GitHub repository based on the uploaded ASL recognition system scripts:

---

```markdown
# ASL Recognition System Using Hand Landmarks

This project is a deep learning-based American Sign Language (ASL) recognition system that uses MediaPipe for hand tracking and a neural network to classify ASL gestures from hand landmarks. It includes tools for data collection, training, and real-time recognition with text-to-speech output.

## Features

- Hand landmark detection using [MediaPipe](https://google.github.io/mediapipe/)
- Data collection tool for generating custom ASL datasets
- Neural network training using TensorFlow/Keras
- Real-time ASL recognition from webcam input
- Text-to-speech output for recognized signs

## Project Structure

```

.
├── asl\_recognition.py     # Real-time ASL recognition and speech
├── data\_collection.py     # Tool to collect ASL gesture data
├── train\_model.py         # Script to train the gesture recognition model
├── utils.py               # Utility functions for data handling
├── data/                  # Directory where gesture data is stored
├── asl\_model.h5           # Trained model file (generated after training)
└── class\_names.npy        # Saved list of class names

````

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/asl-recognition.git
   cd asl-recognition
````

2. **Install Dependencies**:
   Make sure you are using Python 3.10. Then install required packages:

   ```bash
   pip install opencv-python mediapipe numpy tensorflow pyttsx3
   ```

3. **Data Collection**:
   Run the script and follow the prompts to collect data:

   ```bash
   python data_collection.py
   ```

4. **Model Training**:
   After collecting enough data, train the model:

   ```bash
   python train_model.py
   ```

5. **Real-Time Recognition**:
   Use your webcam to detect and recognize ASL gestures:

   ```bash
   python asl_recognition.py
   ```

## Requirements

* Python 3.10
* OpenCV 4.7+
* MediaPipe 0.9.3+
* NumPy 1.23+
* TensorFlow 2.12+
* pyttsx3 (for text-to-speech)

## Notes

* Press `q` to quit during both data collection and recognition.
* Ensure good lighting and clear hand visibility for accurate results.
* Trained model (`asl_model.h5`) and `class_names.npy` must be present in the root directory for recognition to work.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgements

* MediaPipe by Google for real-time hand tracking.
* TensorFlow and Keras for model building.

