# Emotion-Adaptive Learning Platform

## Real-Time Student Focus Detection using Java & OpenCV

An intelligent online learning platform that detects student focus in real time using Computer Vision techniques. The system uses a webcam to analyze facial and eye movements and determines whether the student is **FOCUSED** or **NOT FOCUSED** during online learning sessions.

---

## Features

* Real-time webcam monitoring
* Face detection using Haar Cascade Classifier
* Eye detection within detected face region
* Focus status identification
* Displays student name dynamically
* Lightweight and efficient implementation
* Supports adaptive online learning environments

---

## Technologies Used

* **Programming Language:** Java
* **Library:** OpenCV
* **Computer Vision:** Haar Cascade Classifiers
* **IDE:** Eclipse
* **Hardware:** Webcam

---

## Project Structure

```bash
fcsdtn/
│
├── FocusDetector.java
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
└── README.md
```

---

## How the System Works

1. The webcam captures live video.
2. Each frame is converted to grayscale.
3. Face detection is performed using Haar Cascade.
4. Eye detection is applied inside the face region.
5. If two or more eyes are detected:

   * Status = FOCUSED
6. Otherwise:

   * Status = NOT FOCUSED
7. The result is displayed in real time.

---

## Focus Detection Logic

```java
if (eyes.toArray().length >= 2) {
    status = "FOCUSED";
} else {
    status = "NOT FOCUSED";
}
```

---

## Requirements

* Java JDK 8 or above
* OpenCV Java Library
* Webcam
* Eclipse IDE (Recommended)

---

## Setup Instructions

### 1. Install OpenCV

Download and configure OpenCV for Java.

### 2. Add OpenCV Library

Add the OpenCV JAR file to your project build path.

### 3. Place XML Files

Ensure the following XML files are inside the project directory:

* `haarcascade_frontalface_default.xml`
* `haarcascade_eye.xml`

### 4. Run the Project

Execute the `FocusDetector.java` file.

---

## Sample Output

* Detects student face in real time
* Displays:

  * Student Name
  * FOCUS Status
* Draws rectangle around detected face

---

## Applications

* Smart Online Learning Platforms
* Virtual Classroom Monitoring
* Student Attention Analysis
* Adaptive Learning Systems
* E-Learning Research

---

## Future Enhancements

* Emotion detection (Happy, Sad, Bored, Stressed)
* Deep Learning-based analysis
* Attendance tracking
* Teacher analytics dashboard
* LMS integration

---

## Conclusion

This project demonstrates a simple and effective real-time focus detection system using Java and OpenCV. It helps improve student engagement and acts as a foundation for advanced emotion-adaptive learning platforms.

---

## Author

**Ghoushenisha Begam J**

---
