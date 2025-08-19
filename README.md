# 📱 SMS Spam Classification using Naive Bayes

This project demonstrates **text classification** on the famous [SMS Spam Collection dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection) using the **Multinomial Naive Bayes algorithm**.  
The goal is to classify SMS messages as either **Ham (not spam)** or **Spam**.

---

## 📊 Dataset
- **Source:** UCI Machine Learning Repository  
- **Size:** 5,572 SMS messages  
- **Classes:**  
  - `ham` → Non-spam message  
  - `spam` → Spam/advertisement message  

Example data:
ham Go until jurong point, crazy.. Available only in bugis...
spam Free entry in 2 a wkly comp to win FA Cup final tkts...


---

## 🚀 Project Workflow
1. Load dataset (`SMSSpamCollection`)
2. Preprocess data (labels → numeric, features → Bag-of-Words using CountVectorizer)
3. Split into training and testing sets
4. Train `MultinomialNB` model
5. Evaluate with:
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

---

## 📈 Results

- **Accuracy:** 96.7%  
- **Confusion Matrix:**


[[937 29]
[ 7 142]]

- **Classification Report:**
          precision    recall  f1-score   support

     ham       0.99      0.97      0.98       966
    spam       0.83      0.95      0.89       149

accuracy                           0.97      1115

macro avg 0.91 0.96 0.93 1115
weighted avg 0.97 0.97 0.97 1115


✅ The model performs very well with ~97% overall accuracy.  

---

## ⚙️ Tech Stack
- Python
- Pandas
- Scikit-learn
- CountVectorizer (Bag-of-Words)

---

## 📂 How to Run
```bash
# Clone the repository
git clone https://github.com/ishanegi5/sms_spam_classification_nb.git

# Navigate to the folder
cd sms_spam_classification_nb

# Install dependencies
pip install -r requirements.txt

# Run the notebook or script

📜 License

This project is open-source and available under the MIT License.
