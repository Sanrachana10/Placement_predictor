# 🎓 Placement Predictor

A Hybrid Ensemble AI system that predicts student placement outcomes using a combination of Machine Learning, Deep Learning, and Transformer-based NLP models.

The system combines RoBERTa, Bidirectional LSTM, SVM, and numerical academic indicators through a weighted soft-voting mechanism to provide accurate placement predictions and identify students who may require additional support.

---

## 🚀 Features

- Placement prediction using AI
- Hybrid Ensemble Architecture
- RoBERTa-based contextual understanding
- BiLSTM sequence modeling
- TF-IDF + SVM baseline classifier
- Numerical profile scoring
- Real-time Streamlit deployment
- Handles class imbalance using SMOTE

---

## 🏗️ Architecture

The system combines four independent prediction signals:

### Expert Model 1
- TF-IDF Vectorization
- Calibrated SVM

### Expert Model 2
- Keras Tokenizer
- Bidirectional LSTM

### Expert Model 3
- RoBERTa Transformer
- Contextual semantic embeddings

### Expert Model 4
- Numerical placement score

Based on:
- CGPA
- Internships
- Coding Skills
- Aptitude Score

### Final Decision

Weighted Soft Voting:

```text
10% SVM
20% BiLSTM
30% RoBERTa
40% Numerical Score
```

A hard rule predicts **Not Placed** if active backlogs exceed 2.

---

## 📊 Dataset

### Student Placement Dataset

- 2500+ student records
- Balanced using SMOTE
- Academic and skill-based features

### Input Features

#### Academic
- Degree
- Branch
- CGPA

#### Career Readiness
- Internships
- Major Projects
- Coding Skill Score
- Aptitude Score
- Active Backlogs

---

## 🤖 Models Used

| Model | Purpose |
|---------|---------|
| SVM | Statistical text classification |
| BiLSTM | Sequential pattern learning |
| RoBERTa | Contextual semantic understanding |
| Ensemble | Final prediction |

---

## 📈 Results

| Model | Accuracy |
|---------|---------|
| SVM | 54.84% |
| BiLSTM | 60.93% |
| RoBERTa | 61.20% |
| Hybrid Ensemble | 81.4% |

### Ensemble Performance

- Accuracy: 81.4%
- F1 Score: 0.82
- ROC-AUC: 0.88

The ensemble significantly outperformed all standalone models.

---

## 🛠️ Tech Stack

### Machine Learning
- Scikit-Learn
- SVM
- SMOTE

### Deep Learning
- TensorFlow
- Keras
- BiLSTM

### NLP
- Hugging Face Transformers
- RoBERTa
- TF-IDF

### Deployment
- Streamlit

### Utilities
- Joblib
- Pandas
- NumPy

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/placement-predictor.git
cd placement-predictor
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run app.py
```

---

## 💻 Usage

1. Enter student details:
   - Degree
   - Branch
   - CGPA
   - Internships
   - Projects
   - Coding Skills
   - Aptitude Score
   - Active Backlogs

2. Click **Predict Placement Status**

3. View:
   - Placement Prediction
   - Placement Probability
   - Confidence Score

---


## 🔮 Future Improvements

- Resume Parsing using OCR and NLP
- Explainable AI using SHAP
- Integration with Career Cell systems
- Real-world placement datasets
- Larger Transformer models (DeBERTa, BERT-large)
- REST API deployment

---

## 👨‍💻 Author

**Sanrachana Singh**

Information Technology Undergraduate, SGSITS Indore

Interests:
- Artificial Intelligence
- Machine Learning
- NLP
- Educational Data Mining
- Backend Development

---

⭐ If you found this project useful, consider giving it a star.
