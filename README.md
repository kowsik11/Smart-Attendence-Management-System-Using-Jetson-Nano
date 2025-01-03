# 🧑‍🏫 Smart Attendance Management System 🎓

This project demonstrates a **Smart Attendance Management System** using **Jetson Nano**. The system utilizes **real-time face detection and recognition** to automate the attendance management process in an academic environment. The project integrates **Haar Cascade models** for nose and eye detection and **autoencoders** for enhancing face recognition accuracy.

## 📑 Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Security and Accuracy Enhancements](#security-and-accuracy-enhancements)
- [Contributing](#contributing)
- [License](#license)

## 📝 Project Description

The **Smart Attendance Management System** automates the process of attendance taking in educational institutions by recognizing faces in real-time. Using the **Jetson Nano** platform, the system captures live video feeds and matches student faces with a database to mark attendance. This system reduces manual errors, enhances security, and provides a more efficient solution for managing large classrooms.

### 🔑 Key Features:
- **Real-Time Face Detection**: Detects faces using the Jetson Nano’s onboard camera.
- **Face Recognition**: Identifies students from a pre-registered dataset using **autoencoders** to improve recognition accuracy.
- **Automated Attendance**: Marks attendance as soon as the student’s face is detected and matched.
- **Database Integration**: Stores attendance data in a local database for easy management and record-keeping.
- **Accuracy Enhancement**: Uses **autoencoders** to increase face recognition accuracy and minimize false positives/negatives.

## 🧠 Features of the System

- **Haar Cascade Face Detection**: Detects faces in the live video feed.
- **Face Recognition with Autoencoders**: Ensures high accuracy in student identification.
- **Automated Attendance Logging**: Logs attendance in real-time based on face matching.
- **User Interface for Administration**: A simple interface to view attendance data, manage the student database, and more.
- **Real-Time Processing**: The system works in real-time to mark attendance as students enter the room.

## 🔧 Technologies Used
- **Hardware**: Jetson Nano
- **Libraries**: OpenCV, Dlib, NumPy, TensorFlow
- **Face Detection**: Haar Cascade (OpenCV)
- **Face Recognition**: Autoencoders (using TensorFlow for model building)
- **Database**: SQLite for attendance record storage
- **Programming Language**: Python

## 🚀 How to Run

### 📥 Prerequisites
Ensure you have the following installed and set up:
- Jetson Nano development board
- Python 3.x
- OpenCV, Dlib, TensorFlow, NumPy, and other necessary libraries

### ⚙️ Installation Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/smart-attendance-management.git
   cd smart-attendance-management

2. Install the required dependencies:
pip install -r requirements.txt

3. Download the pre-trained Haar Cascade model and other necessary files (if not included):
# Download Haar Cascade XML file
wget https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml

4. Set up the database for student records:
python setup_database.py

5. Run the application:
python attendance_system.py

6. Open the camera feed, and as faces are detected, the system will mark attendance and store it in the database.

🛡️ Security and Accuracy Enhancements
Face Recognition Accuracy: Autoencoders are used to reduce false positives and improve recognition rates.
Secure Data Storage: Attendance records are securely stored in a local SQLite database to prevent unauthorized access.
Real-Time Processing: The system runs in real-time, ensuring up-to-date attendance tracking without manual intervention.






