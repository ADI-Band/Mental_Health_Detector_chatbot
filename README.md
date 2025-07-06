# Real-Time Facial Emotion Detection and Mental Health Response System

This project is a two-part real-time system that uses computer vision and deep learning to detect facial emotions and provide relevant mental health feedback. It consists of:

- **`Cnn(final).ipynb`**: Captures live webcam feed, detects faces using Haar Cascade, predicts mood using a trained CNN model, and transmits the dominant mood.
- **`CNN_Reciever.ipynb`**: Receives the detected mood and generates mental health tips or responses accordingly.

---

## 📌 Features

- Real-time face detection using OpenCV and Haar cascade.
- Emotion classification using a Convolutional Neural Network (`model.h5`).
- Tracks dominant mood via statistical mode.
- Sends mood data to a response system for generating tailored feedback.

---

## 🔧 Requirements

Install dependencies using:

```bash
pip install opencv-python tensorflow numpy matplotlib

🚀 How to Run
1. Clone the repository (if hosted):
git clone https://github.com/your-username/emotion-mh-system.git
cd emotion-mh-system

2. Place all files in the same directory:
Cnn(final).ipynb
CNN_Reciever.ipynb
model.h5
haarcascade_frontalface_default.xml

3. Run the system
Step 1: Detect mood
Open and run Cnn(final).ipynb in Jupyter Notebook. This will:
 - Open your webcam
 - Detect faces
 - Classify the emotion
 - Store and send the most frequent mood

Step 2: Respond based on mood
Open and run CNN_Reciever.ipynb. This notebook:
 - Waits for mood data
 - Generates appropriate mental health responses or suggestions based on the emotion
Note: You must replace the Hugging Face access token in CNN_Reciever.ipynb with your own for the API to work.

🎯 Use Cases
1. Mood-aware AI mental health assistants
2. Real-time emotion tracking systems
3. Emotion-based interaction interfaces for well-being platforms
