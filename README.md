# 🖥️ Face Recognition Based Attendance System

A **Flask + OpenCV + KNN** based real-time face recognition attendance system that:

✅ Registers new users with webcam-captured images  
✅ Trains a KNN classifier for face recognition  
✅ Takes attendance automatically when a recognized user appears  
✅ Stores attendance with timestamp in daily CSV logs  
✅ Displays live attendance records via a clean web interface

---

## 🚀 Features

✅ **User Registration** using webcam (capture multiple face images automatically)  
✅ **Real-time Face Detection & Recognition** using Haar Cascades and KNN  
✅ **CSV Attendance Logging** with Name, Roll, and Timestamp  
✅ **Web Dashboard** to view current day's attendance  
✅ Automatic **model retraining** when a new user is added  
✅ Stores **attendance per day** (`Attendance/Attendance-mm_dd_yy.csv`)  
✅ Stores **face images per user** in organized folders  

---

## 📦 Installation

1️⃣ **Clone the repository:**


git clone https://github.com/yourusername/face-recognition-attendance.git
cd face-recognition-attendance

**⚙️ How It Works**
✅ Face Detection: Uses Haar Cascade to detect faces from webcam frames
✅ Registration:

Navigate to Add User page

Enter username and user ID

Capture nimgs face images automatically using webcam

Stores them in static/faces/{username_userid}/

**✅ Training:**

After adding a user, the system retrains the KNN classifier using newly added faces

Stores the trained model as static/face_recognition_model.pkl

**✅ Taking Attendance:**

Navigate to Take Attendance

The webcam opens, detects faces, and identifies them using the trained KNN model

Marks attendance with timestamp in Attendance/Attendance-mm_dd_yy.csv

**✅ Dashboard:**

View the Name, Roll, Time of attendees for the current day

Displays total registered users

**🧠 Use Cases**
✅ Automated attendance in colleges, coaching centers, offices

✅ Face recognition learning project for beginners in ML and CV

✅ Demonstration for final year projects or hackathons

**📈 Improvements to Consider**
✅ Switch from KNN to deep learning models (FaceNet, dlib) for higher accuracy

✅ Integrate database (SQLite, MongoDB) for scalable storage

✅ Enable mobile camera or IP camera support

✅ Add notification on attendance capture

✅ Attendance analytics and reports
