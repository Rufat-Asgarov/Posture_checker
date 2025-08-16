# Posture + Screen Distance Monitor (Windows, Python)

A lightweight **Windows tray application** that helps you maintain healthy screen habits:

### ✨ Features
- **Posture & Distance Monitoring** using your webcam
- **First‑time forced calibration** to set a personal baseline
- **Immediate alerts** when you get too close to the screen (sound + Windows toast notification)
- **Sensitivity slider** (5% → 70% closer than baseline)
- **Good posture streak rewards** (toast after consistent streaks)
- **Auto‑saved config & logs** (`.json` stored next to the app)
- **Runs silently in the background** as a tray icon
- **No mediapipe, no heavy DNN models** — pure OpenCV cascade ensemble (Haar + LBP + Profile + eye validation)

### 🛠 Installation
```bash
pip install opencv-python pystray pillow win10toast
python posture_monitor_no_mediapipe_gui.py
```

### 📦 Build as EXE
```bash
pip install pyinstaller
pyinstaller --onefile --noconsole --name PostureMonitor posture_monitor_no_mediapipe_gui.py
```

### 📋 Why it’s unusual
This project blends **personal ergonomics + gamification** into a tiny background app — promoting healthier habits while you work or game.
