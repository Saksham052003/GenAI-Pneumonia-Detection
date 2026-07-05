# GenAI-Pneumonia-Detection

**GenAI-Pneumonia-Detection** is an end-to-end web application for pneumonia detection from Chest X-ray images using Deep Learning and Google Gemini.

---

## Live Demo

| Resource | Link |
|----------|------|
| Frontend | https://pneumonia-detection-theta.vercel.app/ |
| Backend API | https://saksham052003-pneumonia-detection-backend.hf.space/ |
| Dataset | https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia |

---

## About the Project

Reading chest X-rays for pneumonia requires medical expertise and can be time-consuming. This project explores how Deep Learning and Generative AI can work together to assist in this process.

GenAI-Pneumonia-Detection is an end-to-end web application for pneumonia detection from chest X-ray images. It combines a deep learning model built with TensorFlow/Keras and pretrained CNN backbones (EfficientNetB0 and DenseNet121) with Google Gemini to generate structured radiology reports. Users can upload a chest X-ray, enter patient information, and receive both a prediction and an AI-generated report through a React-based web interface.

The project consists of a React frontend, a Flask backend, and a trained TensorFlow/Keras model deployed separately from the application.

---

## Features

- Detects Pneumonia from Chest X-ray images
- Generates AI-based radiology reports using Google Gemini
- Displays prediction confidence
- Collects patient information before analysis
- Drag-and-drop image upload
- Responsive React interface
- REST API built with Flask
- Ready for cloud deployment

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| Frontend | React.js, HTML5, CSS3 |
| Backend | Flask, Python |
| Deep Learning | TensorFlow, Keras, EfficientNetB0, DenseNet121 |
| Computer Vision | OpenCV, Pillow |
| Data Processing | NumPy, Pandas |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Generative AI | Google Gemini API |
| Development | Google Colab, VS Code, Git, GitHub |
| Deployment | Vercel, Hugging Face Spaces |

---

## Model Highlights

- EfficientNetB0 and DenseNet121 used as feature extractors.
- Feature fusion with channel attention for improved representation learning.
- Binary classification (Normal vs Pneumonia).
- Trained using TensorFlow/Keras.
- Grad-CAM used for model interpretability during experimentation.
- Google Gemini used for automated radiology report generation.

---

## How it Works

1. Upload a Chest X-ray image.
2. Enter patient details.
3. The backend preprocesses the image.
4. The trained TensorFlow/Keras model predicts the disease.
5. The confidence score is calculated.
6. Google Gemini generates a structured medical report.
7. The frontend displays the prediction and AI-generated report.

---

## Dataset

The model was trained using the **Chest X-ray Pneumonia Dataset** by Paul Mooney available on Kaggle.

https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

---

## Running the Project

### Backend

```bash
pip install -r requirements.txt
python app.py
```

Create a `.env` file

```env
GEMINI_API_KEY=YOUR_API_KEY
MODEL_URL=YOUR_MODEL_URL
```

---

### Frontend

```bash
npm install
npm start
```

Create a `.env` file

```env
REACT_APP_API_URL=http://localhost:5000
```

---
