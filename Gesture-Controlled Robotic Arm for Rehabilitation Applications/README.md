# Gesture-Controlled Robotic Arm for Rehabilitation Applications

**Grade:** 77/100  
**Summary:** This project delivers a **fully runnable codebase** for a real-time gesture recognition and robotic control system, driving a **Dobot Magician robotic arm**.  
It integrates **computer vision, machine learning, and robotic control** to enable intuitive human–robot interaction, with direct potential in **rehabilitation therapy**.

---

## Repository Structure
Gesture-Controlled-Robotic-Arm/
│
├─ Codes/ # FULL project source code
│ ├─ hand_tracking.py # MediaPipe 21 landmark detection
│ ├─ finger_counting.py # Real-time finger counter
│ ├─ multi_hand_distance.py # Euclidean distance between hands
│ ├─ virtual_drawing.py # Drawing & shape recognition
│ ├─ realtime_control_dobot.py # Direct robot control via gestures
│ ├─ models/
│ │ ├─ keras_model.h5 # Custom CNN gesture classifier
│ │ └─ labels.txt # Gesture label definitions
│ └─ utils/ # Helper functions & modules
│
├─ Demo/ # Demonstration videos
│ ├─ Finger Counting(Hand Recognition).mp4
│ ├─ Finger Counting(Multi-Hand Recognition).mp4
│ ├─ Hand Distance Measurement(Multi-Hand Recognition).mp4
│ ├─ Real-time Gesture Control-Gripper.mp4
│ ├─ Real-time Gesture Control-Suction Cup.mp4
│ └─ Virtual Drawing(Gesture Recognition).mp4
│
└─ Dissertation.pdf # Full technical report



**Codes/** contains the **complete implementation** used to achieve the results in the report and demos.  
All modules are runnable and documented, covering **gesture recognition, CNN classification, and robotic actuation**.

---

## Features
- Real-time **hand tracking** (MediaPipe, 21 landmarks).  
- **CNN gesture classifier** (Keras, Teachable Machine export).  
- **Finger counting** (single & multi-hand).  
- **Multi-hand distance measurement**.  
- **Virtual drawing & recognition** → circle, line, "X", then robotic reproduction.  
- **Direct robot control** (Dobot Magician) with gestures for gripper & suction cup.  

---

## Technical Stack
- **Languages:** Python 3.9+  
- **Libraries:** OpenCV, MediaPipe, CVZone, TensorFlow/Keras, NumPy, PySerial  
- **Hardware:** Dobot Magician (gripper / suction cup), RGB camera  
- **ML Model:** Custom CNN (`keras_model.h5` + `labels.txt`)  

---

## Setup & Run
### 1. Install dependencies
```bash
pip install opencv-python mediapipe cvzone tensorflow numpy pyserial

### 2. Dobot SDK
Place DobotDllType.py and DLLs in Codes/ (or add to PYTHONPATH).

Connect Dobot Magician via USB at 115200 baud.

### 3. Run modules

cd Codes/

# Hand tracking
python hand_tracking.py

# Finger counting
python finger_counting.py

# Multi-hand distance
python multi_hand_distance.py

# Virtual drawing + robotic drawing
python virtual_drawing.py

# Real-time Dobot control
python realtime_control_dobot.py


# Demos
1. Finger Counting – Single Hand

2. Finger Counting – Multi-Hand

3. Hand Distance Measurement

4. Virtual Drawing & Robotic Reproduction

5. Real-time Gesture Control – Gripper

6. Real-time Gesture Control – Suction Cup

(All videos available in /Demo/.)

# Performance
- Accuracy: >90% gesture recognition in tests.

- Latency: Runs in real time on laptop CPU.

- Robustness: Works under cluttered backgrounds and low-light conditions.

# Applications
- Rehabilitation Therapy: Enables therapists to guide patient exercises while enforcing safe motion ranges.

- Human–Robot Interaction: Natural hands-free robot control.

- STEM Education: Demonstrates full integration of AI + robotics.

This repository includes the full working codebase, demos, and dissertation report, showing the complete pipeline from gesture perception → classification → robotic execution.
