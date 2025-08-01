# 📧 Spam vs Ham Classification using TF-IDF

A machine learning project to classify emails as **spam** or **ham** using text preprocessing and **TF-IDF vectorization**.

## 📌 Objective

To accurately detect spam emails using logistic regression on vectorized message content, even with an **imbalanced dataset**.

---

## 🧾 Dataset

- **Features**:  
  - `Category`: `spam` or `ham`  
  - `Message`: The text of the email  
- **Total samples**: 5572  
- **Distribution**:  
  - Ham: 4825  
  - Spam: 747  

➡️ The dataset is **imbalanced**, so evaluation is done using  **recall**, not just accuracy.

---

## 🧪 Tools & Libraries

- **Python**
- `pandas`, `numpy`
- `scikit-learn`
- `Tokenization for text preprocessing`
- `TfidfVectorizer` (for converting text to numerical features)
- `Logistic Regression`

---

## ⚙️ Approach

1. **Preprocessing**:
   - Label encoding `Category` (ham=0, spam=1)
   - Splitting into train/test sets

2. **Feature Extraction**:
   - `TfidfVectorizer(min_df=1, stop_words='english', lowercase=True)`
   - Transformed both `X_train` and `X_test`

3. **Modeling**:
   - Used **Logistic Regression**
   - Evaluated on training and test data using:
     - Recall
    
---

## 📊 Results

| **Metric**              | **Value**     |
|-------------------------|---------------|
| Training Accuracy       | 96.74%        |
| Test Accuracy           | 96.05%        |
| Recall (Spam Detection) | 99.3%         |
| F1 Score                | 99.1%         |


---

## 👩‍💻 Author

**Tanya Chauhan** 
[LinkedIn](https://www.linkedin.com/in/tanya-chauhan-99a5aa355/)  
📍 New Delhi  
✉️ tanyachauhan084@gmail.com
