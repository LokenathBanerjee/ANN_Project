# 📊 Customer Churn Prediction Using Artificial Neural Network (ANN)

## 📌 Project Overview

Customer churn is a critical problem for businesses, as retaining existing customers is often more cost-effective than acquiring new ones.  
This project implements an **Artificial Neural Network (ANN)** model to predict whether a customer is likely to **stay with** or **leave** a company based on historical customer data.

The system is divided into three main components:

1. **Model Building & Training**
2. **Prediction Pipeline**
3. **Streamlit Web Application**

---

## 🧠 1. Model Building & Training

- The model is built using **TensorFlow (Keras)**.
- A **Churn Dataset** is used, containing both numerical and categorical features.
- Data preprocessing includes:
  - Handling categorical variables using **ColumnTransformer**
  - Feature scaling
- The trained ANN model is saved in **`.h5`** format.
- The preprocessing pipeline is serialized using **pickle** for reuse during prediction.

### 📁 Relevant Files

- `eda.ipynb` – Exploratory Data Analysis  
- `pred3.ipynb` – Model training and evaluation  
- `Saved_Model/churn_model.h5` – Trained ANN model  
- `Saved_Model/preprocessor.pkl` – Saved preprocessing pipeline  

---

## 🔍 2. Prediction Module

- User input is collected in real time.
- Input data is transformed using the **same preprocessing pipeline** used during training.
- The ANN model outputs a **churn probability**:
  - **> 0.5** → Customer likely to churn  
  - **≤ 0.5** → Customer likely to stay  

This ensures consistency and reliability between training and inference.

---

## 🌐 3. Streamlit Web Application

An interactive web interface is developed using **Streamlit**, allowing users to:

- Enter customer details (credit score, age, geography, balance, etc.)
- View churn probability instantly
- Receive a clear **churn / not-churn** decision

The Streamlit application:
- Loads the trained ANN model  
- Loads the saved preprocessing pipeline  
- Accepts user inputs and displays results in real time  

### ▶️ To Run the Application

```bash
streamlit run app.py
| Category             | Technologies                |
| -------------------- | --------------------------- |
| Programming Language | Python                      |
| Data Analysis        | Pandas, NumPy               |
| Visualization        | Matplotlib, Seaborn         |
| Machine Learning     | Scikit-learn                |
| Deep Learning        | TensorFlow (Keras)          |
| Model Persistence    | Pickle                      |
| Web Framework        | Streamlit                   |
| Development Tools    | Jupyter Notebook, IPykernel |
| Monitoring           | TensorBoard                 |

📄 All dependencies are listed in requirements.txt
```

## 📁 Project Structure
```
├── app.py                     # Streamlit application
├── eda.ipynb                  # Exploratory Data Analysis
├── pred3.ipynb                # Model training & prediction
├── requirements.txt           # Project dependencies
├── Saved_Model/
│   ├── churn_model.h5         # Trained ANN model
│   └── preprocessor.pkl       # Saved preprocessing pipeline
✅ Conclusion
```
This project demonstrates an end-to-end machine learning system, from data analysis and ANN model training to deployment using a web interface.

## 🚀 Future Enhancements:-

Add model evaluation metrics in the UI

Deploy the app on Streamlit Cloud

Enhance feature engineering

Experiment with different ANN architectures

## 👤 Author Details

Author: Lokenath Banerjee
Degree: B.Tech in Computer Science Engineering (Artificial Intelligence & Machine Learning)

Institute: Haldia Institute of Technology

Location: West Bengal, India

### 🚀 Connect With Me

📧 Email: lokenathb2005@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/lokenath-banerjee-53a95928b/

🐙 GitHub: https://github.com/LokenathBanerjee/

