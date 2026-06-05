# 🩺 Diabetes Prediction using Deep Learning (FNN)

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![Accuracy](https://img.shields.io/badge/Accuracy-94%25-success.svg)](#)

## 📌 Project Overview
This project focuses on building a robust **Feedforward Neural Network (FNN)** to predict the onset of diabetes based on medical records. By analyzing various patient features such as insulin levels, BMI, blood pressure, and genetic markers, the model achieves a high classification accuracy, demonstrating the power of Deep Learning in early medical diagnosis and healthcare analytics.

## 🛠️ Tech Stack & Libraries
* **Data Manipulation & Analysis:** `Pandas`, `NumPy`
* **Deep Learning Framework:** `TensorFlow`, `Keras`
* **Machine Learning & Preprocessing:** `Scikit-Learn` (StandardScaler, train_test_split, metrics)
* **Data Visualization:** `Matplotlib`, `Seaborn`

## 📊 Dataset & Preprocessing
* **Source:** Kaggle (ankitbatra1210/diabetes-dataset) - 70,000 patient records.
* **Data Cleaning:** Identified missing medical indicators (recorded as `0` for BMI, Blood Pressure, etc.) and imputed them using the column mean to maintain data integrity.
* **Feature Engineering:** Transformed descriptive target strings into binary outcomes (`1` for Diabetic, `0` for Non-Diabetic).
* **Encoding & Scaling:** Applied One-Hot Encoding for 20 categorical variables and used `StandardScaler` to normalize numerical features for optimal neural network convergence.

## 🧠 Model Architecture
A Feedforward Neural Network optimized for tabular data classification:
* **Input Layer:** Scaled numerical and encoded categorical features.
* **Hidden Layers:** Two Dense layers (128 and 64 units) with `ReLU` activation.
* **Regularization:** `Dropout` layers (0.3 rate) applied after each hidden layer to prevent overfitting.
* **Output Layer:** Single unit with `Sigmoid` activation for binary probability prediction.
* **Compilation:** `Adam` optimizer and `binary_crossentropy` loss function.

## 📈 Key Results & Performance
The model was trained for 100 epochs, achieving outstanding generalization on the unseen test data (14,000 samples).

* **Test Accuracy:** `94%`
* **Test Loss:** `0.1365`
* **Precision & Recall:** 
  * Class 1 (Diabetic): Precision **0.94**, Recall **0.96**
  * Class 0 (Healthy): Precision **0.93**, Recall **0.91**

### Visualizations
*(Note: Upload your plots to the `images` folder to display them here)*

<p align="center">
  <img src="images/accuracy_plot.png" alt="Model Accuracy" width="45%">
  &nbsp; &nbsp; &nbsp;
  <img src="images/loss_plot.png" alt="Model Loss" width="45%">
</p>

<p align="center">
  <img src="images/confusion_matrix.png" alt="Confusion Matrix" width="60%">
</p>

## 💡 Business Impact & Conclusion
With an F1-Score of **0.95** for positive cases, this model proves highly reliable in minimizing false negatives (failing to identify a sick patient). Implementing such an AI-driven approach in clinical settings can significantly aid doctors in early diagnosis, prioritize high-risk patients, and optimize healthcare resources.

## 👥 Team
* **Rezk Youssef Rezk**
* **Salma Ahmed AbdElshahid**

---
⭐ *Feel free to explore the code in the `.ipynb` file. If you find this project helpful, a star to the repository is highly appreciated!*
