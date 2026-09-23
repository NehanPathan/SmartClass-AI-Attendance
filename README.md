# 🎓 SmartClass AI Attendance

> An AI-powered smart classroom attendance system using **Face Recognition** and **Voice Recognition** for automated and efficient student attendance.

## 🌐 Live Demo

🚀 **Try the application:**  
https://smartclass-attendance.streamlit.app/

---

## 📌 About

**SmartClass AI Attendance** is an AI-based classroom attendance management system designed to automate the traditional attendance process.

The system combines **face recognition** and **voice recognition** to verify students and record their attendance. It also provides class creation, QR-based class joining, student management, and attendance tracking through an interactive Streamlit interface.

The project is designed as an academic/educational project to demonstrate the practical use of **AI, biometric recognition, and cloud-based data management** in classroom environments.

---

## ✨ Features

- 🎭 **Face Recognition**  
  Identify and verify students using facial features.

- 🎙️ **Voice Recognition**  
  Verify students using voice embeddings.

- 📋 **Automatic Attendance**  
  Record attendance after successful identity verification.

- 👨‍🎓 **Student Management**  
  Manage student registration and class enrollment.

- 🏫 **Class Management**  
  Create and manage classroom sessions.

- 📱 **QR Code Class Joining**  
  Students can join a class using a unique class code or QR code.

- 📊 **Attendance Records**  
  Store and manage student attendance history.

- ☁️ **Cloud Database**  
  Use Supabase for storing application data.

- 🔐 **Authentication & Security**  
  Password hashing and authentication using bcrypt.

- ⚡ **Interactive Web Interface**  
  Built with Streamlit for a simple and responsive user experience.

---

## 🧠 AI Components

### Face Recognition

The face-recognition component uses:

- `dlib-bin`
- `face_recognition_models`
- `scikit-learn`

The system uses facial features to identify registered students during attendance.

### Voice Recognition

The voice-recognition component uses:

- `librosa`
- `resemblyzer`

Voice recordings are processed to generate voice embeddings that can be used for student verification.

---

## 🛠️ Tech Stack

### Programming Language

- Python

### Frontend / UI

- Streamlit

### Face Recognition

- dlib
- face_recognition_models
- scikit-learn

### Voice Recognition

- Librosa
- Resemblyzer

### Data Processing

- NumPy
- Pandas

### Database

- Supabase

### Authentication

- bcrypt

### Utilities

- Segno
- Pillow

---

## 🏗️ Project Architecture

```text
                         ┌─────────────────────┐
                         │      Streamlit      │
                         │     Web Interface   │
                         └──────────┬──────────┘
                                    │
                  ┌─────────────────┴─────────────────┐
                  │                                   │
                  ▼                                   ▼
        ┌──────────────────┐                ┌──────────────────┐
        │ Face Recognition │                │ Voice Recognition│
        │                  │                │                  │
        │ dlib             │                │ Librosa          │
        │ Face Models      │                │ Resemblyzer      │
        │ Scikit-learn     │                │ Voice Embeddings │
        └────────┬─────────┘                └────────┬─────────┘
                 │                                   │
                 └────────────────┬──────────────────┘
                                  ▼
                         ┌─────────────────┐
                         │    Attendance   │
                         │    Processing   │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │     Supabase    │
                         │     Database    │
                         └─────────────────┘
