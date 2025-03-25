# Disaster-Prediction-and-Management-Using-Machine-Learning
This project implements a machine learning pipeline for classifying disasters: Wildfire, Flood, and Earthquake. It combines a neural network as a feature extractor with XGBoost for classification.
## 📂 Dataset

- Source: EM-DAT (https://www.emdat.be/)
- Format: Excel (.xlsx)
- Filtered for disaster types: `Wildfire`, `Flood`, and `Earthquake`.

> Please place your dataset at the path specified in `main.py`, or modify the path accordingly.

## 🧠 Model Overview

1. **Preprocessing:**
   - Missing value imputation
   - Label encoding
   - Standardization
   - SMOTE for class balancing

2. **Neural Network:**
   - Multi-layer perceptron for feature embedding
   - Trained using PyTorch

3. **Classifier:**
   - XGBoost with hyperparameter tuning (via `GridSearchCV`)

4. **Evaluation:**
   - Accuracy, confusion matrix, classification report
   - ROC curves with AUC
   - 3D embedding visualization

## 🛠️ How to Run

```bash
pip install -r requirements.txt
python main.py
```

## 📈 Output

- Model accuracy and classification report
- Confusion matrix heatmap
- ROC curve for each class
- 3D scatter plot of neural network embeddings

---

## 🔁 Notes

- Update the `file_path` variable in `main.py` to point to your EM-DAT dataset location.
- You can modify the number of epochs, batch size, or XGBoost parameters as needed.
