# 🩺 AI-Based Pneumonia Detection from Chest X-rays

An end-to-end Deep Learning application that detects **Pneumonia** from Chest X-ray images using **TensorFlow**, **EfficientNetB0**, and **Streamlit**. The project includes model training, evaluation, explainability using **Grad-CAM**, and a web application for real-time prediction.

---

## 📌 Features

- Chest X-ray image classification
- Transfer Learning with EfficientNetB0
- Image preprocessing and augmentation
- Model training and fine-tuning
- Performance evaluation
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve
- Grad-CAM Explainability
- Interactive Streamlit Web Application

---

## 🛠 Tech Stack

- Python 3.12
- TensorFlow / Keras
- EfficientNetB0
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV
- Pillow
- Streamlit

---

## 📂 Project Structure

```text
medical-imaging-pneumonia-detection/

├── app.py
├── config.py
├── requirements.txt
├── README.md
│
├── data/
│   └── chest_xray/
│
├── models/
│   └── final_model.keras
│
├── reports/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   ├── precision_recall_curve.png
│   └── gradcam.png
│
├── src/
│   ├── dataset.py
│   ├── model.py
│   ├── train.py
│   ├── evaluate.py
│   ├── predict.py
│   └── gradcam.py
```

---

## 🧠 Model

**Architecture:** EfficientNetB0

**Transfer Learning:** ImageNet Pretrained Weights

**Input Size:** 224 × 224 RGB

**Loss Function:** Binary Crossentropy

**Optimizer:** Adam

**Output Classes**

- NORMAL
- PNEUMONIA

---

## 📊 Model Performance

| Metric | Value |
|---------|------:|
| Accuracy | 62% |
| ROC-AUC | 0.74 |

### Classification Report

| Class | Precision | Recall | F1-score |
|--------|----------:|-------:|---------:|
| NORMAL | 0.00 | 0.00 | 0.00 |
| PNEUMONIA | 0.62 | 1.00 | 0.77 |

---

## 📈 Results

### Confusion Matrix

> <img width="772" height="672" alt="image" src="https://github.com/user-attachments/assets/e4c6b13d-8628-4916-a448-ac7342a3612d" />


---


### Grad-CAM Visualization

> <img width="867" height="737" alt="image" src="https://github.com/user-attachments/assets/9fe4bb79-8126-446c-b268-d4fbcf80f4e9" />


---

## 💻 Streamlit Web App

The application allows users to:

- Upload a Chest X-ray image
- Predict NORMAL or PNEUMONIA
- Display confidence score
- View an intuitive web interface

Run locally: 

```bash
python -m streamlit run app.py
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/<your-username>/medical-imaging-pneumonia-detection.git
```

Move into the project directory

```bash
cd medical-imaging-pneumonia-detection
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate the virtual environment

Windows

```bash
.venv\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### Train the model

```bash
python src/train.py
```

### Evaluate the model

```bash
python src/evaluate.py
```

### Predict a single image

```bash
python src/predict.py
```

### Generate Grad-CAM

```bash
python src/gradcam.py
```

### Launch the web application

```bash
python -m streamlit run app.py
```

---

## 🚧 Current Limitations

- The model tends to overpredict the **PNEUMONIA** class due to dataset imbalance.
- Additional fine-tuning and threshold optimisation could improve performance.
- This project is intended for **educational and research purposes only** and is **not** a medical diagnostic tool.

---

## 🔮 Future Improvements

- Better class balancing
- Hyperparameter tuning
- Advanced data augmentation
- Additional CNN architectures
- Multi-class lung disease classification
- Model deployment using Docker and cloud services

---

## 👩‍💻 Author

**Drashti Kamodia**

MBBS | Healthcare AI | Medical Imaging | Deep Learning

This project is licensed under the MIT License.# medical-imaging-pneumonia-detection
AI-powered pneumonia detection from chest X-ray images using TensorFlow, EfficientNetB0, Streamlit, and Grad-CAM explainability.
