# 🤟 Sign Language Recognition using Deep Learning

This project detects and translates **American Sign Language (ASL)** hand gestures into spoken letters using **real-time video**, a **Convolutional Neural Network (CNN)** model, and **text-to-speech (TTS)**. It supports both **single and two-hand gestures**, including complex signs like the letter **Z**.

---

## 🔧 Features

- 📷 Real-time webcam-based gesture recognition
- 🧠 Trained CNN model using ASL image dataset
- 🔤 Recognizes A-Z and 0-9 (36 classes)
- 🔈 Text-to-speech audio output using `pyttsx3`
- ✌️ Two-hand gesture support (e.g., for "Z")
- ⚡ Fast and lightweight prediction loop
- 🧼 Data preprocessing notebook included

---

## 📁 Project Structure

SignLanguageRecognition/
│
├── model/
│ └── asl_model.h5 # Trained CNN model
├── sign_language_detect.py # Real-time gesture recognition script
├── data_preprocessing.ipynb # Notebook for dataset loading & training
├── requirements.txt # List of required Python packages
├── sample_images/ # Example hand signs (optional)
└── README.md # Project info (you're here!)


---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/VinaySMVS/sign-language-detection.git
cd sign-language-detection

2. Install Requirements
pip install -r requirements.txt

3. Run the Detection Script
python sign_language_detect.py

Your webcam will start, and the recognized ASL letters will be displayed and spoken.

4. Train the Model (Optional)
jupyter notebook data_preprocessing.ipynb

Follow the steps in the notebook to preprocess data and train the model. The final model will be saved as asl_model.h5.
🧠 Model Info
Input size: 64x64 RGB images

Model: Convolutional Neural Network (CNN)

Output: 36 softmax units (26 letters + 10 digits)

Optimizer: Adam

Loss: Categorical Crossentropy

Validation Accuracy: > 99%

🎯 Dataset
You can use any open ASL dataset such as:

Kaggle's ASL Alphabet

Custom images captured using webcam

Each class should have folders of labeled images (A-Z, 0-9).
📦 Requirements
These are listed in requirements.txt, but for reference:

opencv-python
tensorflow
numpy
pyttsx3
mediapipe

Install with:
pip install -r requirements.txt
🧠 Future Enhancements
Add sentence formation using time-sequenced gestures

Upload web demo using Streamlit or Flask

Include regional sign languages (e.g., ISL)

Mobile app integration with TensorFlow Lite

Gesture smoothing to reduce flickering predictions

👤 Author
Vinay SMVS
🔗 GitHub
📧 Email: vcpdeloli@example.com