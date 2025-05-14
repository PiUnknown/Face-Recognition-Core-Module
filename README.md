# 🧠 Face Recognition Core Module

A raw, no-fluff, lightweight face recognition module using OpenCV's Haar Cascade and the LBPH face recognizer. Built for real-time facial recognition via webcam with modular and minimal design — no GUI layers, no distractions.

---

## 🚀 Features

- Real-time face **detection** using Haar Cascades
- Face **recognition** using OpenCV's LBPH algorithm
- Custom dataset generation via webcam
- Lightweight design focused on core logic
- Basic visualization using `cv2.imshow()` (for debugging only)

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** OpenCV (`cv2`), NumPy
- **Model:** Haar Cascade Classifier + LBPH Recognizer
- **Input:** Webcam
- **Output:** Live window with detected face name (or "not recognized")

---

## 📁 Project Structure
├── create_data.py # Capture face images and save dataset
├── face_recognize.py # Real-time face recognition
├── haarcascade_frontalface_default.xml # Haar model for face detection
└── datasets/ # Auto-created folder for captured face data

---

## 📸 Dataset Creation

Run this to capture images of a new person:

```bash
python create_data.py
```

- Enter the person’s name when prompted.
- 200 images will be saved under datasets/<name>/.

---

## 🔍 Face Recognition (Live)

Once the dataset is ready, start real-time recognition:

```bash
python face_recognize.py
```

- Recognized faces will show the name and confidence score.
- Unknown faces will be labeled "not recognized".

---

## ⚙️ Dependencies
Make sure you have these installed:

```bash
pip install opencv-python numpy
pip install opencv-contrib-python
```

---

## 📚 Credits
This project was built using knowledge and inspiration from various open-source resources and tutorials, including:
- [Face Recognition using LBPH – PyImageSearch](https://pyimagesearch.com)
- [OpenCV LBPH Projects on GitHub](https://github.com/topics/lbph)

---

