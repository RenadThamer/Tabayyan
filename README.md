# Tabayyan (تبيّن) - Detecting and Preventing Online Job Posting Scams with AI-Powered NLP

Tabayyan is an AI-powered security framework and web platform designed to detect and prevent online recruitment fraud and phishing URLs using Natural Language Processing (NLP), Machine Learning, and Deep Learning.

---

## 🌟 Key Features
- **Dual-Layer Verification Pipeline:** 
  1. Inspects the legitimacy of recruitment URLs across 32 phishing indicators (IP usage, subdomain depth, HTTPS security, domain age).
  2. Analyzes textual content, semantic structures, and deceptive language patterns within job descriptions.
- **Weighted Ensemble Architecture:** Integrates predictions from **Random Forest (RF)** and **Convolutional Neural Networks (CNN)** weighted dynamically via TF-IDF statistical properties for maximum reliability.
- **Explainable AI (XAI):** Incorporates interpretability tools (including **LIME** for CNN and permutation importance) to reveal the key textual features driving classification decisions (e.g., job requirements and company profile credibility).
- **User History & Authentication:** Seamlessly integrates with Google Firebase (Auth & Cloud Firestore) to track and store user scans securely.

---

## 🔬 Methodology & Experimental Highlights
- **Datasets:** EMSCAD (17,880 job postings) & Phishing Websites Dataset (11,055 URLs, 32 attributes).
- **NLP Preprocessing:** Text normalization, custom stop-word removal, and WordNet Lemmatization.
- **Feature Extraction:** High-dimensional TF-IDF vectorization (yielding up to 13,275 preprocessed text features).
- **Class Balancing:** Addressed severe real/fake class imbalance using **SMOTE** and **Oversampling**.
- **Model Benchmark:** Rigorously evaluated across 6 extensive experiments comparing:
  - Machine Learning: Random Forest (RF), Support Vector Machine (SVM), XGBoost, Logistic Regression (LR).
  - Deep Learning: Multi-Layer Perceptron (MLP), Convolutional Neural Networks (CNN).
  - Outcome: The RF model achieved up to 100% accuracy under full preprocessed oversampling, with CNN demonstrating robust deep-learning performance above 98.9% accuracy.

---

## 🛠️ Tech Stack
- **Machine Learning & Deep Learning:** Random Forest, CNN (Convolutional Neural Networks), SVM, XGBoost, SMOTE.
- **Natural Language Processing (NLP):** NLTK (WordNet), TF-IDF Vectorizer, Scikit-learn, LIME.
- **Backend & Serving:** Python (Flask), Pickle.
- **Database & Auth:** Google Firebase (Firestore & Authentication).
- **Frontend:** HTML5, CSS3, JavaScript (UI prototyped via Figma).

---

## 🚀 Getting Started

### 1. Installation
Clone the repository and install the dependencies:
git clone https://github.com/RenadThamer/Tabayyan.git
cd Tabayyan
pip install -r requirements.txt

### 2. Run Application
python app.py

Open your browser and navigate to:
http://127.0.0.1:5000

---

## 👥 Team Members:
- **Renad Albogami**
- **Shahad Aldeiji**
- **Rola Alzahrani**
- **Bushra Alzeghabi**
- **Taif Alharbi**
