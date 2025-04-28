Face Recognition Attendance System

A simple Flask-based web application that allows users to:

Register their faces using a webcam 📸

Mark attendance by recognizing faces

Save attendance records in an Excel sheet (attendance.xlsx)




face-attendance/
│
├── app.py                # Main Flask app
├── known_faces/          # Folder where registered face images are stored
├── attendance.xlsx       # Excel file where attendance is saved
├── templates/
│   ├── home.html         # Home page
│   ├── register.html     # Face Registration page
│   ├── attendance.html   # Attendance marking page
│   └── success.html      # Success or error messages
└── static/
    └── (optional css/js files)




Requirements
Python 3.7+

Flask

OpenCV

face_recognition

pandas



How it works
Register Face:

Enter your name.

The app captures your face and saves it under known_faces/.

Mark Attendance:

The system matches live webcam input with registered faces.

If a match is found, your name and date are recorded in attendance.xlsx.