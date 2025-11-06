# 🎧 MoodBeats — Emotion-Based Music Recommender

MoodBeats is a real-time emotion-based music recommendation system that detects facial expressions using **MediaPipe + Deep Learning**, classifies emotions, and automatically opens mood-appropriate YouTube music based on detected emotion and user language preference.

---

## 🚀 Features
- Real-time facial emotion recognition via webcam  
- Custom dataset collection (your own expressions)  
- Emotion classification using TensorFlow/Keras  
- MediaPipe Holistic for landmark extraction  
- Streamlit-based interface  
- Opens YouTube music based on detected emotion & user preference   

---

## 🧠 Tech Stack
| Category | Technology |
|---|---|
Language | Python  
ML Framework | TensorFlow / Keras  
Face Tracking | MediaPipe Holistic  
UI | Streamlit + WebRTC  
Others | NumPy, OpenCV  

---

## 📂 Project Structure

MoodBeats/
│── data_collection.py # Collects facial landmarks + saves dataset
│── data_training.py # Trains NN & saves model + labels
│── final.py # Streamlit app for real-time emotion-music interaction
│── model.h5 # Generated model after training
│── labels.npy # Generated emotion label map


## 📦 Installation & Setup

### Clone Repo

git clone https://github.com/mandeep793/MoodBeats.git
cd MoodBeats

Requirements needed to be installed --- pip install opencv-python mediapipe tensorflow streamlit streamlit-webrtc numpy


🏁 Usage Guide

Step 1: Collect Emotion Data   -
python data_collection.py
Enter emotion label (e.g., happy, sad, angry)
Make expressions while webcam captures frames
Repeats for each emotion → Saves .npy dataset

Step 2: Train Your Model
python data_training.py
Generates:
model.h5
labels.npy

Step 3: Run the App
streamlit run final.py

Select:

🎭 Emotion detected automatically

🌐 Language (Punjabi/Hindi/English)

🎵 Artist preference

App opens relevant YouTube songs like:

https://www.youtube.com/results?search_query=punjabi+happy+song+ap+dhillon

🎯 Example Emotions Supported
Happy, Sad, Angry, Neutral 
(More can be added by collecting extra data)


🔮 Future Enhancements
Spotify / YouTube API Integration, Deployment on Streamlit Cloud / HuggingFace, FER/AffectNet dataset for higher accuracy, In-app music player, Emotion timeline graph


👤 Author
Mandeep Kaur
B.E. CSE — Chandigarh University
