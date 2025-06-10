# 📁 Project Structure: Gesture-Controlled Light System

# 1. hello.py
# This script handles gesture detection and sends signals to controller.py

# 2. controller.py
# This script controls the Arduino-connected LEDs via pyfirmata

# 3. requirements.txt
opencv-python
cvzone
pyfirmata

# 4. README.md

# Gesture-Controlled Light System 🖐️💡

A gesture-controlled lighting system built using Python, OpenCV, Arduino UNO (SMD), and pyFirmata. The system detects hand gestures through a webcam and lights up LEDs on the Arduino based on finger combinations.

## 🔧 Tech Stack
- Python
- OpenCV
- cvzone
- pyFirmata
- Arduino UNO (SMD)
- StandardFirmata firmware

## 📸 How It Works
- Webcam captures hand in real-time
- OpenCV + cvzone detect fingers raised
- Finger count is passed to controller.py
- controller.py maps gestures to GPIO pins (LEDs)
- Arduino lights up LEDs accordingly

## 📂 Files
- `hello.py`: gesture detection
- `controller.py`: LED control
- `requirements.txt`: dependencies
- `media/`: images & videos 

## 🧪 Setup Instructions
1. Upload `StandardFirmata` to Arduino UNO using Arduino IDE:
   - File > Examples > Firmata > StandardFirmata > Upload
2. Connect Arduino via USB
3. Clone this repository
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Run `hello.py`

## 📷 Demo 
Youtube video :https://youtube.com/shorts/kPgqk_JEXTA?si=Mxxy86zFihLvk3_p

## 🙌 Built by Shravani Patil
Connect: [LinkedIn](https://www.linkedin.com/in/shravani-patil-38791b286/)

---

# 💡 Notes
- Make sure Arduino IDE is **closed** when running Python code
- Use correct COM port (e.g., 'COM3', 'COM6')
- Check pin numbers and wiring if LEDs don’t respond
