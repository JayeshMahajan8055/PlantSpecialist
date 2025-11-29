🌱 PlantDoc - Plant Disease Detection System
A CNN-Based Deep Learning Model powered computer vision system that identifies plant diseases from leaf images using a custom Convolutional Neural Network (CNN). The solution is designed for real-time agricultural diagnostics and can be deployed as a web application for farmers and agritech platforms.

🚀 Features
Custom-built CNN architecture optimized for multi-class plant disease classification
Comprehensive dataset preprocessing: normalization, augmentation, and stratified splitting
Real-time Flask API for leaf image uploads and instant predictions
Grad-CAM explainability to highlight infected regions in the image
High-accuracy model trained on PlantVillage dataset
Production-ready pipeline with model saving (SavedModel format)
🏗️ System Architecture
User Upload → Preprocessing → CNN Model
                              ↓
                        Class Prediction
                              ↓
                   Confidence Score + Heatmap (Grad-CAM)
🧠 Model Overview
Custom CNN with:

Convolution + MaxPooling layers
Batch Normalization
Dropout regularization
Adam optimizer with LR scheduling
Trained on 80/10/10 split

Achieves strong generalization on unseen leaf images

🛠️ Tech Stack
Deep Learning: TensorFlow, Keras
Backend: Flask
Data Processing: NumPy, Pandas
Visualization: Matplotlib, Grad-CAM
Deployment: Python, Virtual Environment
📦 Installation
git clone https://github.com/<username>/plant-disease-detection.git
cd plant-disease-detection

pip install -r requirements.txt
▶️ Usage
1️⃣ Run the Flask App
python app.py
2️⃣ Upload a leaf image via the UI
The model will return:

Predicted disease name
Confidence score
Grad-CAM heatmap for explainability
📊 Dataset
PlantVillage Dataset

54,000+ leaf images
38 plant disease categories
Healthy + diseased classes
(You may add dataset link if you upload on your repo.)

📈 Results
High test accuracy
Robust inference under variations (lighting, orientation)
Grad-CAM maps validate disease-focused interpretation
🔮 Future Improvements
Deploy model via Docker + FastAPI
Convert model to TensorFlow Lite for mobile/edge devices
Add YOLO-based disease localization
Add real-time field monitoring using drone imagery
