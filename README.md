# MorphyDex – Malnutrition Classification (CNN + TFLite + Flutter)

MorphyDex is an end-to-end system that detects **malnourished vs healthy** status from a person’s image using a custom-trained **Convolutional Neural Network (CNN)**.  
The model is converted to **TensorFlow Lite (TFLite)** and deployed inside a **Flutter mobile application** so all predictions run **on-device**, without needing internet.

---

## 🚀 Features

- 📱 Cross-platform Flutter app (Android/iOS)
- 🧠 Custom CNN model for malnutrition classification
- ⚡ Fast, offline inference using TensorFlow Lite
- 📸 Camera / gallery image input
- 🧩 Clean project structure (data, models, view, view_model)
- 🔥 Firebase-ready configuration
- 🟢 Output: *Healthy* or *Malnourished*

---

## 🧠 Machine Learning Model

Model development happens in Python using TensorFlow/Keras.

**Notebook & model files:**

```text
jupyter notebook/
├─ malnutrition_classification_model.ipynb   # CNN training & export
├─ model.tflite                              # Exported TFLite model
└─ label.txt                                 # Class labels (e.g., Healthy, Malnourished)
MorphyDex/
│
├─ assets/
│   ├─ banner/
│   ├─ images/
│   └─ model/
│       ├─ model.tflite      # TFLite model used in the app
│       └─ label.txt         # Class label names
│
├─ jupyter notebook/
│   ├─ malnutrition_classification_model.ipynb
│   ├─ model.tflite
│   └─ label.txt
│
├─ lib/
│   ├─ data/
│   ├─ helper/
│   ├─ models/
│   ├─ res/
│   ├─ utils/
│   ├─ view/
│   ├─ view_model/
│   └─ main.dart             # Flutter entry point
│
├─ android/
├─ ios/
├─ firebase.json
├─ pubspec.yaml
└─ README.md
