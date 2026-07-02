## 🤖 Intelligent Hybrid Recommendation System

> **An AI-powered recommendation system that goes beyond keyword matching by combining NLP, personality compatibility (MBTI), location-based scoring, and adaptive feedback learning to generate personalized profile recommendations.**

---

## 📌 Project Overview

Traditional recommendation systems often rely on simple keyword matching, which fails to understand the true meaning behind user profiles. This project addresses that limitation by combining **Natural Language Processing (NLP)**, **MBTI personality compatibility**, **location-based preferences**, and an **adaptive feedback mechanism** to deliver more intelligent and meaningful recommendations.

The system analyzes professional summaries, personality traits, and user interactions to calculate compatibility scores and continuously improve recommendation quality over time.

---

## ✨ Key Features

- 🔍 Semantic profile matching using **TF-IDF** and **Cosine Similarity**
- 🧠 MBTI personality compatibility scoring
- 📍 Location-based preference matching
- ⚖️ Hybrid weighted scoring algorithm
- 🔄 Adaptive feedback loop that updates recommendation weights
- 📊 Top-N personalized recommendations
- 📈 Beginner-friendly implementation in **Google Colab**

---

## 🏗️ System Architecture

The recommendation pipeline consists of three major modules:

### **Module 1 – Understanding Layer**
- Text preprocessing
- TF-IDF Vectorization
- Cosine Similarity Calculation

### **Module 2 – Logic Layer**
Calculates compatibility using a weighted hybrid formula:

```
Total Score =
(w1 × Text Similarity)
+ (w2 × MBTI Compatibility)
+ (w3 × Location Score)
```

Default Weights:

- Text Similarity → 50%
- MBTI Compatibility → 30%
- Location → 20%

### **Module 3 – Adaptive Feedback Layer**
The recommendation engine learns from user feedback.

- ✅ Accept → reinforces current weights
- ❌ Reject → adjusts weights to improve future recommendations

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| IDE | Google Colab |
| NLP | TF-IDF |
| Machine Learning | Scikit-learn |
| Data Handling | Pandas, NumPy |
| Similarity | Cosine Similarity |
| Dataset | Custom CSV Dataset |
| Visualization | Architecture Diagram |

---

## 📂 Repository Structure

```
📦 intelligent-hybrid-recommendation-system
│
├── Major_Project.ipynb
├── users_50_profiles.csv
├── match_feedback.csv
├── Project_Architecture.png
├── Project_Documentation.pdf
└── README.md
```

---

## 📊 Dataset

The project uses two custom datasets.

### **users_50_profiles.csv**

Contains profile information of 50 users including:

- User ID
- Name
- Professional Summary
- About Me
- MBTI Personality Type
- Location

### **match_feedback.csv**

Stores user interaction history including:

- User ID
- Recommended User
- Accept / Reject Feedback

---

## 🚀 How It Works

1. Load user profiles.
2. Combine profile text fields.
3. Convert text into vectors using TF-IDF.
4. Compute semantic similarity using Cosine Similarity.
5. Calculate MBTI compatibility.
6. Calculate location score.
7. Generate a weighted compatibility score.
8. Rank recommendations.
9. Learn from user feedback and adjust weights.

---

## 📈 Sample Output

For every user, the system generates:

- Top recommended profiles
- Compatibility percentage
- Dynamic scoring using adaptive weights

Example:

```
Top Matches for User U001

1. Vivek Nair      → 85%
2. Sachin Patel    → 85%
3. Deepak Singh    → 85%
4. Rakesh Nanda    → 85%
5. Khushi Jain     → 62.94%
```

---

## 📷 Project Architecture

The repository includes a visual architecture diagram explaining the complete workflow of the recommendation engine.

---

## 📽️ Project Resources

Complete project resources are available here:

### 📂 Google Drive

Notebook, datasets, documentation, and project explanation video:

**🔗 https://drive.google.com/drive/folders/1PeYI7dizLN0HlzBgvr3b_maRkWDhcdd5**

---

## 🎯 Learning Outcomes

Through this project I gained practical experience in:

- Natural Language Processing
- Recommendation Systems
- Feature Engineering
- Similarity Measurement
- Adaptive Learning
- Python Development
- Google Colab
- Data Preprocessing

---

## 🔮 Future Improvements

- Replace TF-IDF with BERT embeddings
- Deploy using Streamlit or Flask
- Add real-time database integration
- Improve feedback learning using Reinforcement Learning
- Build a web-based recommendation dashboard

---

## 👩‍💻 Author

**Yukti Dubey**

B.Tech Student | AI & Machine Learning Enthusiast

If you found this project interesting, feel free to ⭐ the repository.

---

> *"Finding the right connections requires understanding people—not just matching keywords."*
