# 💤 Real-Time Drowsiness Detection System

A real-time **driver drowsiness detection system** built using Python and computer vision.  
The system monitors eye closure and yawning behavior through a live webcam feed and triggers voice alerts when fatigue indicators cross defined thresholds.

---

## 📌 Project Overview

Drowsiness is a major cause of road accidents and often goes unnoticed until it becomes dangerous.  
This project focuses on **early fatigue detection** by analyzing facial landmarks in real time and providing timely voice alerts to keep the driver alert.

The system uses **Eye Aspect Ratio (EAR)** to detect prolonged eye closure and **Mouth Aspect Ratio (MAR)** to detect yawning.  
If drowsiness persists or **three consecutive yawns** are detected, a voice alert is triggered.

---

## ⚙️ Key Features

- Real-time face detection using webcam  
- Eye closure detection using Eye Aspect Ratio (EAR)  
- Yawn detection using Mouth Aspect Ratio (MAR)  
- Voice alert after sustained eye closure or **3 consecutive yawns**  
- Cooldown mechanism to prevent repeated alerts  
- On-screen metrics panel displaying:
  - EAR value  
  - Yawn state and yawn count  
  - Drowsiness percentage  
  - Face detection status  
  - FPS (performance monitoring)

---

## 🧠 Technologies Used

- Python  
- OpenCV  
- MediaPipe Face Mesh  
- NumPy  
- Windows Text-to-Speech (SAPI)

---

## 🧮 How the System Works

1. Captures live video from the webcam.  
2. Detects facial landmarks using MediaPipe Face Mesh.  
3. Calculates:
   - **EAR (Eye Aspect Ratio)** for eye closure detection  
   - **MAR (Mouth Aspect Ratio)** for yawn detection  
4. Tracks duration and frequency of fatigue indicators.  
5. Triggers a voice alert when:
   - Eyes remain closed beyond a set duration, or  
   - Three consecutive yawns are detected.  
6. Displays real-time visual feedback and system metrics on screen.

---

## ⚙️ Threshold Configuration

The following parameters can be tuned based on camera quality, lighting conditions, and distance:

- `EYE_THRESH` → Eye closure sensitivity  
- `MOUTH_THRESH` → Yawn detection sensitivity  
- `DROWSY_TIME_LIMIT` → Minimum eye-closed duration (seconds)  
- `YAWN_TIME_LIMIT` → Minimum mouth-open duration (seconds)  
- `ALERT_COOLDOWN` → Delay between alerts (seconds)

---

## 🏁 Conclusion

This project demonstrates how computer vision can be applied to real-world safety problems.  
By combining facial landmark analysis with time-based thresholds, the system reliably detects early signs of fatigue and provides timely alerts.

The implementation emphasizes **real-time performance**, **practical alert handling**, and **system stability**, making it a strong foundation for further enhancements and real-world deployment.

---

## 📈 Future Enhancements

- Improve detection accuracy in low-light environments  
- Add blink rate and head pose analysis  
- Store fatigue events for long-term monitoring  
- Cross-platform text-to-speech support  
- Mobile or embedded system deployment  

---

## 🙏 Acknowledgements

Special thanks to **Innomatics Research Labs** for providing a supportive learning environment.  
Grateful to my trainer **Mr. Nagaraju Ekkirala** and mentor **Mohammad Afroz** for their continuous guidance and feedback throughout this project.

---

## 👨‍💻 Author

**Sai B**  
Computer Science Engineer | Python & Computer Vision Enthusiast  


---

## 📬 Feedback & Contributions

Feedback and suggestions are welcome.  
Feel free to connect or raise an issue for discussion.
