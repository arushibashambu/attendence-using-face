# Attendance System Using Face Recognition

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview
The **Attendance System Using Face Recognition** is a computer vision-based system that automates attendance tracking using facial recognition. It captures live video feeds from a camera, detects faces, and matches them with pre-registered faces to mark attendance. This project aims to provide a contactless and efficient way to manage attendance for institutions, workplaces, and events.

## Features
- **Face Detection**: Detects faces in real-time using the camera.
- **Face Recognition**: Recognizes registered faces and marks attendance automatically.
- **Attendance Logging**: Stores attendance data in a CSV file or database for easy access and review.
- **Multiple User Support**: Can recognize and track the attendance of multiple individuals in real-time.
- **User Registration**: Allows users to register their face with a unique ID for attendance purposes.
- **Real-time Attendance**: Continuously updates the attendance status as people are recognized.

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - OpenCV (for real-time face detection and recognition)
  - dlib (for face embeddings and recognition)
  - Face_recognition library (for easier face comparison and matching)
  - NumPy (for data manipulation)
  - Pandas (for managing attendance data)
- **Hardware**: A webcam or external camera
- **IDE**: Jupyter Notebook, PyCharm, or any Python-compatible IDE

## Setup Instructions

### Prerequisites
- Python 3.x
- Required Python libraries (listed in `requirements.txt`)

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/anrao0037/Attendance-System-Using-Face-Recognition.git
   ```

2. **Install Required Libraries**:
   Navigate to the project directory and install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. **Camera Setup**:
   Ensure that your system’s camera is functional or connect an external camera to capture live video.

4. **Face Registration**:
   Register the faces of users by running the `register_faces.py` script. Capture and store images for each user with a unique identifier.

## Usage

1. **Register Faces**:
   - Run the `register_faces.py` script to capture and register faces. This will create a database of face encodings to be used for recognition:
   ```bash
   python register_faces.py
   ```
   - Follow the on-screen prompts to assign a unique ID or name to each user.

2. **Start Attendance System**:
   - Run the `attendance.py` script to start the attendance tracking system:
   ```bash
   python attendance.py
   ```
   - The system will automatically detect faces and match them against the registered faces. Once a face is recognized, the attendance will be marked, and a log will be created.

3. **View Attendance Logs**:
   - After running the system, check the `attendance.csv` file (or database) for a detailed log of attendance. This file will contain user names/IDs along with the timestamp of when their attendance was marked.

## Contributing
Contributions are welcome! If you would like to contribute, please fork the repository and submit a pull request. Ensure that your changes align with the project’s objectives and coding standards.

