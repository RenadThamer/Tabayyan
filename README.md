# Tabayyan (تبيّن) - Detecting and Preventing Online Job Posting Scams with AI-Powered NLP

Tabayyan is an AI-powered security framework and web platform designed to detect and prevent online recruitment fraud and phishing URLs using Natural Language Processing (NLP), Machine Learning, and Deep Learning.

---

## 🌟 Key Features
- **Dual-Layer Verification Pipeline:** 
  1. Inspects recruitment URLs against phishing indicators and verified domain whitelists (e.g., official government and educational domains).
  2. Analyzes textual content, semantic structures, and deceptive language cues within job descriptions.
- **Weighted Ensemble Architecture:** Deploys a hybrid voting mechanism that dynamically integrates predictions from **Random Forest (RF)** and **Convolutional Neural Networks (CNN)** weighted via TF-IDF statistical properties.
- **Explainable AI (XAI):** Built upon experimental feature importance insights (including LIME for CNN) to focus detection on high-risk fields like job requirements, company profiles, and location context.
- **User History & Authentication:** Seamlessly integrates with Google Firebase (Authentication & Cloud Firestore) to track and store user scans securely.

---

## 🔬 Methodology & Experimental Highlights
- **Datasets:** EMSCAD (17,880 job postings) & Phishing Websites Dataset (11,055 URLs, 32 attributes).
- **NLP Preprocessing:** Text normalization, stop-word removal, POS tagging, and WordNet Lemmatization.
- **Feature Extraction:** High-dimensional TF-IDF vectorization (generating up to 13,275 preprocessed features).
- **Class Balancing:** Addressed real/fake data imbalance using **SMOTE** and **Oversampling**.
- **Model Selection:** Rigorously evaluated across 6 experimental iterations; the deployed architecture combines the optimal Oversampling models of **Random Forest** (100% benchmark score) and **CNN** (98.9% benchmark score) into a single decision threshold.

---

## 🛠️ Tech Stack
- **Machine Learning & Deep Learning:** Random Forest, CNN (Convolutional Neural Networks), SMOTE, Oversampling.
- **Natural Language Processing (NLP):** NLTK (WordNet & POS Tagging), TF-IDF Vectorizer, Scikit-learn.
- **Backend & Serving:** Python (Flask), Pickle.
- **Database & Auth:** Google Firebase (Cloud Firestore & Firebase Authentication).
- **Frontend:** HTML5, CSS3, JavaScript (UI prototyped via Figma).

---

## 🚀 Getting Started

### 1. Clone the Repository
git clone https://github.com/RenadThamer/Tabayyan.git
cd Tabayyan

### 2. Install Dependencies
pip install -r requirements.txt

### 3. Run the Application
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
