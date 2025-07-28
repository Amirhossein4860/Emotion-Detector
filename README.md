# Emotion-Detector
A complete NLP pipeline for detecting emotions in text using classic ML models (MLP, Decision Tree, Logistic Regression) and various linguistic features (TF-IDF, Word2Vec, POS tagging). Includes preprocessing, feature engineering, evaluation, and real-time prediction support.

# 😃 Emotion Detection from Text using Machine Learning

This repository showcases a full Natural Language Processing (NLP) pipeline for detecting **emotions in text** using classic machine learning models. From data preprocessing to real-time deployment, the project highlights feature extraction techniques, model evaluation, and user-friendly execution through a graphical interface and `.exe` app.

---

## 🧠 Project Overview

Emotion recognition from text has impactful applications in sentiment analysis, mental health monitoring, customer service, and intelligent chatbots. This project classifies emotional states such as:

- 😊 Joy
- 😢 Sadness
- 😠 Anger
- 😱 Fear
- 😐 Neutral

I built and trained ML models on labeled emotion datasets using linguistic features like TF-IDF, Word2Vec, and POS tagging.

---

## 📂 Dataset
The dataset consists of short English text phrases, each labeled with one of several emotion categories such as joy, sadness, fear, anger, or neutral.

| Column Name | Description |
|-------------|-------------|
| `Text`      | The raw text input (e.g., sentence or phrase) |
| `Emotion`   | The labeled emotion for each sample (e.g., joy, anger, fear) |

## 🔄 Data Processing Workflow

### 1️⃣ **Dataset Preparation**
- Load the labeled emotion dataset.
- Shuffle and split data for training and evaluation.
- Handle class imbalance if present.

### 2️⃣ **Text Preprocessing**
- Convert text to lowercase, remove stopwords and special characters.
- Tokenization and lemmatization.
- POS tagging for syntactic feature extraction.

### 3️⃣ **Feature Engineering**
- Generate text features using:
  - TF-IDF Vectorization
  - Bag-of-Words
  - Word2Vec Embeddings
  - POS tag counts

### 4️⃣ **Model Development & Training**
- Trained and compared the following machine learning models:
  - Logistic Regression
  - Decision Tree Classifier
  - Multi-Layer Perceptron (MLP)
- Used pipelines and `joblib` to save and reuse models.
- Visualized performance with confusion matrices and classification reports.

### 5️⃣ **Model Evaluation**
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score

## 🚀 How to Run the Project

### **1️⃣ Clone the Repository**
- Clone this repository to your local machine:
```sh
$ git clone https://github.com/Amirhossein4860/Emotion-Detector.git
$ cd Emotion-Detector
```
### **2️⃣ Install Dependencies**
- Make sure all required libraries are installed:
```sh
$ pip install -r requirements.txt
```

### **3️⃣ Run the Jupyter Notebook**
- Start the Jupyter Notebook to explore and run the project:
```sh
$ jupyter notebook NLP_Emotion_Detection.ipynb
```
Open NLP_Emotion_Detection.ipynb and execute the cells step-by-step.

### **4️⃣ Run the GUI App (Optional)**
- For real-time emotion prediction with a user interface:
```sh
$ python app.py
```

### **5️⃣ Use the EXE File (No Python Required)**
- Download the .exe from the Releases page and run the app directly.


## 📊 Results & Insights

### 🏆 Best-Performing Model
- The Logistic Regression model achieved the highest accuracy and balanced performance across all metrics. It is efficient, interpretable, and well-suited for real-time emotion detection.
