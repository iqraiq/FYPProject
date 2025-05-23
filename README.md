# AI-Guide

This repository contains a demo application built using a custom dataset of 5 speakers from Virtual University (VU). The application demonstrates three key modules:

- 🗣️ **Voice Cloning & TTS** using [Coqui TTS]
- 🎞️ **Lip Syncing** using [Wav2Lip]

---

## 📁 Dataset

We created a custom dataset with manually recorded audio and video samples from 5 VU speakers. Each speaker has clean audio samples for training TTS and video recordings for lip sync evaluation.

- 🎤 Audio: Clean WAV files  
- 🎥 Video: Front-facing videos with clear lip movement

---

## 🧩 Project Modules

### 1. Voice Cloning & Text-to-Speech (TTS)
- **Tool**: [Coqui TTS] 
- **Dataset Used**: Custom 5-speaker dataset  
- **Output**: Realistic synthetic speech mimicking each speaker

### 2. Lip Syncing
- **Tool**: [Wav2Lip]
- **Dataset Used**: Custom 5-speaker dataset 
- **Input**: A video file + generated audio  
- **Output**: A lip-synced video where the speaker appears to say the generated text

## 📌 How It Works (AI Guide Flow)

1. ✍️ **Enter Text**  
   The user enters any text they want to convert into a lecture or guide.

2. 🧠 **Voice Cloning with Selected Speaker**  
   The text is converted into speech using a selected VU speaker’s cloned voice.

3. 👄 **Lip Syncing**  
   A selected speaker video is lip-synced with the generated voice using Wav2Lip.

4. 🌆 **Change Background (Optional)**  
   You can change the background of the video to match the lecture environment.

5. 📥 **Download Final Video**  
   The final lip-synced, background-changed video is ready for download and learning!


---
## 🧠 Technologies Used

- 🤖 **Deep Learning Models**  
  We trained TTS and Voice Cloning and Lipsynch models using deep learning on our 5-speaker dataset.

- 📱 **Mobile App**  
  The frontend is developed in **React Native** to make it easy to use on mobile devices.

- 🛠️ **Flask API**  
  A **Flask** server acts as a bridge between the mobile app and the **deep learning model.**

- ☁️ **Model Hosting in Kaggle Notebook**  
  The trained models are hosted and run inside **Kaggle Notebooks**, and the mobile app calls the Flask API to process the text, generate audio, and sync lips.

---

