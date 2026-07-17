# Hand Gesture Controlled Audio Alert System

## 📌 Overview

This project is a **real-time hand gesture recognition system** built using **Python, OpenCV, MediaPipe, and Pygame**. It detects the number of fingers shown to a webcam and plays a corresponding audio alert.

The application uses **MediaPipe Hands** to track hand landmarks, counts the raised fingers, and triggers different sound files for specific gestures. This project demonstrates the integration of computer vision with multimedia applications.

---

## 🚀 Features

* Real-time hand tracking using a webcam
* Detects up to **2 hands** simultaneously
* Counts the number of raised fingers
* Plays different audio alerts based on finger count
* Displays detected hand landmarks
* Shows the finger count on the video feed
* Prevents repeated audio playback for the same gesture
* Exit using **Q** or **Esc**

---

## 🛠️ Technologies Used

* Python
* OpenCV
* MediaPipe
* Pygame

---

## 📂 Project Structure

```text
├── hand_gesture_alert.py
├── alert1.mp3
├── alert2.mp3
├── alert3.mp3
├── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/hand-gesture-audio-alert.git
cd hand-gesture-audio-alert
```

### 2️⃣ Create a Virtual Environment (Optional)

```bash
python -m venv venv
```

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install opencv-python mediapipe pygame
```

---

## ▶️ How to Run

Run the application:

```bash
python hand_gesture_alert.py
```

The webcam will start automatically.

### Gesture Mapping

| Fingers Detected | Action             |
| ---------------- | ------------------ |
| 1 Finger         | Plays `alert1.mp3` |
| 2 Fingers        | Plays `alert2.mp3` |
| 3 Fingers        | Plays `alert3.mp3` |
| Other Gestures   | No audio           |

Press **Q** or **Esc** to close the application.

---

## 📸 Output

The application displays:

* Live webcam feed
* Hand landmarks
* Finger count on the screen
* Audio alerts based on detected gestures

---

## 🧠 How It Works

1. Captures video from the webcam using OpenCV.
2. Converts each frame from BGR to RGB.
3. Uses **MediaPipe Hands** to detect hand landmarks.
4. Counts the number of raised fingers.
5. Displays the finger count on the video feed.
6. Plays the corresponding audio file when a new gesture is detected.
7. Avoids repeated playback for the same gesture until the hand changes.

---

## 🧩 Concepts Covered

* Computer Vision
* Hand Landmark Detection
* Gesture Recognition
* Finger Counting Algorithm
* Real-Time Video Processing
* Audio Playback with Pygame
* Event Handling
* OpenCV Image Processing

---

## ⏱️ Performance

| Metric           | Complexity                                                  |
| ---------------- | ----------------------------------------------------------- |
| Finger Counting  | **O(1)**                                                    |
| Frame Processing | **O(n)** *(depends on frame size and MediaPipe processing)* |
| Memory Usage     | **O(1)**                                                    |

---

## 🔮 Future Improvements

* Detect custom hand gestures
* Control smart home devices using gestures
* Volume control with finger distance
* Media player controls (Play/Pause, Next, Previous)
* Gesture-based presentation controller
* Gesture-controlled mouse
* Support for custom audio mapping
* Add FPS counter
* Improve thumb detection accuracy
* GUI for configuring gesture actions

---

## 🎯 Learning Outcomes

After completing this project, you will understand:

* How MediaPipe detects hand landmarks
* Real-time webcam processing using OpenCV
* Finger counting using landmark positions
* Playing audio using Pygame
* Integrating computer vision with multimedia
* Building real-time AI-based gesture applications

---

## 👨‍💻 Author

**Pranay Jadhao**

Electronics & Telecommunication Engineer

Aspiring Software Engineer | Computer Vision | Python | AI & Machine Learning | Embedded Systems

---

## 📄 License

This project is open-source and available for educational and learning purposes.
