# 👁️ Real-Time Eye Gaze Recognition and Media Player Control

A real-time gaze-controlled media player system that uses facial landmarks and pupil tracking for hands-free video interaction. Built using Python, OpenCV, and dlib.

## 👨‍💻 Author
**Abhishek Tyagi**  
Roll No: 42370211217  
Delhi Institute of Tool Engineering (DITE)  
Project under CS50x AI - Harvard University  
📜 [Certificate Link](https://cs50.harvard.edu/certificates/cdea1963-1535-4aef-be8e-d285f8a4f2e4)

## 📽️ Demo Video
[📺 Watch the project in action](https://youtu.be/DKxA6mvGz5w)

## 📦 Features

- Eye region detection using dlib 68-point facial landmarks
- Iris center detection using image thresholding and centroiding
- Blink detection with Eye Aspect Ratio (EAR)
- Gaze-based control of media functions (Play, Pause, Forward, Rewind)
- Calibration system for personalized screen mapping
- Works with standard laptop webcams (~26 FPS real-time performance)

## 🧠 Technical Summary

- **Libraries Used**: `OpenCV`, `Dlib`, `NumPy`, `imutils`
- **Algorithm**:
  - Face and eye detection → ROI extraction
  - Iris thresholding + morphological ops → contour → centroid
  - Eye aspect ratio (EAR) → blink detection
  - Gaze zones mapped to control signals
- **Pipeline**: Modular queue-based threading for real-time frame processing
- **Calibration**: 9-point screen calibration with dynamic ratio mapping

## 🧪 Installation

### Clone this Repository
```bash
git clone https://github.com/AbhishekTyagi404/Deep-Learning-Python.git
cd Deep-Learning-Python/Gaze_Recognition_Media_Player
