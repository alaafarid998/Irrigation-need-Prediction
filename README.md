# Irrigation-need-Prediction
# 🌱 Irrigation Need Prediction

A deep learning model that predicts whether a crop needs **Low**, **Medium**, or **High** irrigation
based on environmental and soil features.

## 📊 Dataset
- Input features: Temperature, Rainfall, Soil Moisture, Wind Speed, Crop Type, Season, etc.
- Target: Irrigation_Need (Low / Medium / High)

## 🧠 Model Architecture
- Neural Network built with TensorFlow/Keras
- Layers: Dense(128) → Dense(64) → Dense(64) → Dense(32) → Dense(3, softmax)
- Optimizer: Adam (lr=0.0001)
- Loss: Sparse Categorical Crossentropy

## ⚙️ Feature Engineering
- Evaporative pressure (Temperature × Wind Speed)
- Dryness vs Moisture ratio
- Available water proxy
- Salt-adjusted moisture

## 🚀 How to Run
1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Open the notebook: `jupyter notebook Irrigation_need_deeplearning_project.ipynb`
4. Run all cells

## 📈 Results
- Achieved 98.13% validation accuracy and 98.41% in test dataset
