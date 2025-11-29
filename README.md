
---

# 🌱 PlantSpecialist – DL-Based Plant Disease Detection System

**PlantSpecialist** is an AI- **deep learning solution** that identifies plant diseases from leaf images using a **custom-built Convolutional Neural Network (CNN)**. Designed for **real-time agricultural diagnostics**, it can be deployed as a **web application** for farmers, agritech platforms, and smart crop monitoring systems.

---

## 🚀 Key Features

* 🔬 Custom CNN model optimized for **multi-class plant disease classification**
* 🧪 Advanced preprocessing pipeline (**normalization, augmentation, stratified split**)
* ⚙️ Real-time **Flask-based web API** for leaf image upload & predictions
* 🔎 **Grad-CAM explainability** to highlight infected regions
* 📈 High model accuracy trained on the **PlantVillage dataset**
* 🛠️ Production-ready pipeline with **model saving (SavedModel format)**

---

## 🏗️ System Architecture

```
User Upload
      ↓
Image Preprocessing
      ↓
CNN Model Inference
      ↓
Prediction + Confidence Score
      ↓
Explainability (Grad-CAM Heatmap)
```

---

## 🧠 Model Overview

The model is based on a **custom CNN architecture** featuring:

* Convolution + MaxPooling layers
* Batch Normalization
* Dropout regularization
* Adam optimizer with learning rate scheduling
* Train–validation–test split: **80% / 10% / 10%**

✔ Achieves **high generalization** on unseen plant leaf images.

---

## 🛠 Tech Stack

| Component       | Technology                      |
| --------------- | ------------------------------- |
| Deep Learning   | TensorFlow, Keras               |
| Backend API     | Flask                           |
| Data Processing | NumPy, Pandas                   |
| Visualization   | Matplotlib, Grad-CAM (heatmaps) |
| Deployment      | Python (virtual environment)    |

---

## 📦 Installation

```bash
git clone https://github.com/<username>/PlantSpecialist.git
cd PlantSpecialist
pip install -r requirements.txt
```

---

## ▶️ Usage

### 1️⃣ Run the Flask App

```bash
python app.py
```

### 2️⃣ Upload a leaf image via the UI

The model returns:
✔ Predicted disease name
✔ Confidence score
✔ Grad-CAM heatmap for explainability

---

## 📊 Dataset

**PlantVillage Dataset**

* 54,000+ plant leaf images
* 38 disease categories
* Includes both **healthy and infected** samples

*(You can provide a dataset link if uploaded in the repository.)*

---

## 📈 Results

* 🔥 High test accuracy
* 📌 Robust predictions under variations (lighting, orientation)
* 🔍 Grad-CAM maps validate disease-focused modeling

---

## 🔮 Future Enhancements

* 🚢 Deploy with **Docker + FastAPI**
* 📱 Convert to **TensorFlow Lite** for edge/mobile deployment
* 🔦 Add **YOLO-based disease localization**
* 🚁 Integration with **drone imagery** for real-time field monitoring

---

## 🧑‍🌾 Impact

✨ PlantSpecialist supports **early disease detection**, helping reduce crop damage and improving agricultural productivity through **AI-driven farming solutions**.

---
