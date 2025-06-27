# 💎 Diamond Price Predictor

A machine learning web application built with **Flask** that predicts the price of a diamond based on key features like **carat, cut, color, and clarity**. This project aims to bring transparency and data-driven accuracy to diamond pricing — especially helpful for both buyers and sellers.

---

## 📽️ Demo

[[Watch the demo](Snapshots and Video/Video)]

---

## 🔍 Problem Statement

Most people are unaware of how diamonds are actually priced. Pricing depends on subtle features that are not easy to estimate without expertise — resulting in many customers overpaying. This project was inspired by a real experience at a jewelry store, where this pricing gap became clear.

---

## ⚙️ Features

- Predicts price of a diamond based on user input  
- Uses machine learning pipeline (`sklearn.pipeline`) for end-to-end processing  
- Built with **Flask** for a clean, interactive UI  
- Handles both numerical and categorical features using `ColumnTransformer`
- Trained on a real-world diamond dataset  
- Achieves **97% accuracy** using **Random Forest Regressor**

---

## 🧪 Tech Stack

- **Python**
- **Flask**
- **pandas**
- **scikit-learn**
- **HTML/CSS (Flask templates)**
- **End-to-End Pipelines**

---

## 🛠️ How to Run the Project

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/diamond-price-predictor.git
   cd diamond-price-predictor

2. Create a virtual environment and activate it

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Flask app

   ```bash
   python application.py
   ```

5. Open your browser and visit `http://127.0.0.1:5000/`

---

## ⚔️ Challenges Faced & How I Tackled Them

### 🧩 1. Handling Categorical Features

* **Challenge**: Features like `cut`, `color`, and `clarity` are not numerical.
* **Solution**: Used `OneHotEncoder` within `ColumnTransformer` to preprocess them inside the pipeline.

### 🔄 2. Overfitting in Initial Models

* **Challenge**: Some models performed well on training but poorly on testing data.
* **Solution**: Used **cross-validation** and **hyperparameter tuning** to reduce overfitting.

### 🔌 3. End-to-End Flexibility

* **Challenge**: Integrating preprocessing and modeling cleanly.
* **Solution**: Used `sklearn.pipeline.Pipeline` for a full preprocessing + training pipeline.

---

## 📈 Results

* Best-performing model: **Random Forest Regressor**
* Achieved **98% accuracy** on both training and test datasets
* Smooth end-to-end workflow with reusable pipeline
* Deployed as an easy-to-use web app with Flask

---
