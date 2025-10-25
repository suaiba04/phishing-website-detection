# 🛡️ Phishing Website Detection using ML

## 📘 Overview
Phishing websites are a prevalent form of social engineering that trick users into revealing sensitive information by mimicking legitimate websites.  
The goal of this project is to **detect phishing websites** by training and evaluating multiple **machine learning** and **deep learning** models on a dataset of both phishing and legitimate URLs.

---

## 📊 Dataset
This project combines **phishing** and **legitimate** URLs from two open-source repositories:

- **Phishing URLs:**  
  Collected from [PhishTank](https://www.phishtank.com/developer_info.php), an open-source platform that maintains a frequently updated database of verified phishing URLs.

- **Legitimate URLs:**  
  Sourced from the [University of New Brunswick (UNB) URL Dataset 2016](https://www.unb.ca/cic/datasets/url-2016.html).  
  The file **`Benign_list_big_final.csv`** (containing **35,300 legitimate URLs**) was used for training.

Both datasets were merged and processed for **feature extraction**, including:
- Lexical-based features (e.g., URL length, presence of special characters)
- Host-based and content-based features (e.g., domain age, WHOIS information, HTML tags)

---

## ⚙️ Models Implemented
The following supervised models were trained and compared:

1. **Decision Tree**  
2. **Random Forest**  
3. **Multilayer Perceptron (MLP)**  
4. **XGBoost**  
5. **Autoencoder Neural Network**  
6. **Support Vector Machine (SVM)**

Each model was trained on extracted features, and its performance was measured on both training and test datasets.

---

## 📈 Model Performance

| **Model**                | **Train Accuracy** | **Test Accuracy** |
|---------------------------|--------------------|-------------------|
| Decision Tree             | 0.814              | 0.803             |
| Random Forest             | 0.821              | 0.821             |
| Multilayer Perceptron     | 0.866              | 0.858             |
| XGBoost                   | 0.868              | 0.858             |
| Autoencoder Neural Net    | 0.759              | 0.755             |
| Support Vector Machine    | 0.802              | 0.803             |

🧠 **Best Performers:**  
- **XGBoost** and **MLP** achieved the highest accuracy (~85.8%), indicating that ensemble learning and deep neural approaches are more effective for this classification problem.



//github.com/<your-username>/phishing-website-detection.git
cd phishing-website-detection
