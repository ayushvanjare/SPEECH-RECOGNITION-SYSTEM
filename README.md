# SPEECH-RECOGNITION-SYSTEM

---

## 📌 About the Project
This project implements a **Speech Recognition System** that converts **spoken audio into text** using Python.

It captures audio from the microphone and processes it using Google’s Speech Recognition API.

---

## ✨ Key Features
- 🎙️ Real-time voice input using microphone  
- 🔊 Converts speech to text instantly  
- 🌐 Uses Google Speech Recognition API  
- ⚡ Simple and lightweight implementation  
- 🧠 Beginner-friendly NLP project  

---

## 🛠️ Tech Stack
- **Language:** Python 3  
- **Libraries:**  
  - SpeechRecognition  
  - PyAudio  
- **API:** Google Speech Recognition  

---

## 📁 Project Structure
📦 Speech-Recognition
┣ 📜 Task_2.ipynb

┣ 📜 audio.wav

┗ 📜 README.md


---

## ⚙️ Setup & Installation
### 1️⃣Install Dependencies

pip install SpeechRecognition

pip install pyaudio

▶️ How It Works

1.The microphone captures audio input

2.Audio is converted into digital format

3.The recognizer processes the audio

4.Google API converts speech → text

5.Output is displayed on the screen

💻 Code Example
import speech_recognition as sr

recognizer = sr.Recognizer()

with sr.Microphone() as source:
    print("Speak something...")
    audio = recognizer.listen(source)

try:
    text = recognizer.recognize_google(audio)
    print("You said:", text)
except:
    print("Error recognizing speech")

▶️ Usage

Run the notebook or script

Speak clearly into your microphone

Wait for processing

View the recognized text output

⚠️ Limitations

Requires internet connection (Google API)

Accuracy depends on microphone quality

Background noise may affect results

Limited support for accents

🔮 Future Enhancements

🚀 Offline speech recognition (Vosk / Whisper)

🚀 Multi-language support

🚀 Noise reduction improvements

🚀 GUI using Tkinter or Streamlit

🚀 Voice command system

