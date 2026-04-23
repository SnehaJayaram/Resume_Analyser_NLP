# 📄 AI Resume Analyser & Ranker (NLP)

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![NLP](https://img.shields.io/badge/Focus-Natural%20Language%20Processing-blueviolet.svg)](#)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)](https://scikit-learn.org/)

## 🎯 Project Objective
In modern recruitment, manually screening hundreds of resumes is a bottleneck. This project implements a **Natural Language Processing (NLP)** pipeline to automate the screening process. By converting text into mathematical vectors, the system calculates a **Similarity Score** between candidate resumes and specific Job Descriptions (JD).

---

## 📊 Visual Proof of Logic
### Candidate Similarity Ranking
![Similarity Scores](./assets/similarity_score_chart.png)
*Figure 1: Visual ranking of candidates based on their alignment with the JD using Cosine Similarity.*

### Skill Distribution Analysis
![Skill Distribution](./assets/skill_distribution.png)
*Figure 2: Automated extraction and frequency analysis of technical keywords across the resume pool.*

---

## 🧠 How it Works (The NLP Pipeline)
1. **Text Extraction:** Using `PyPDF2` to extract raw text from PDF resumes.
2. **Preprocessing:** - **Tokenization:** Breaking text into individual words.
   - **Stopword Removal:** Removing common words (a, the, is) that don't add value.
   - **Normalization:** Lowercasing and cleaning punctuation.
3. **Vectorization (TF-IDF):** - Uses *Term Frequency-Inverse Document Frequency* to give higher weight to rare, technical keywords (e.g., "TensorFlow", "Kubernetes") over common ones.
4. **Ranking (Cosine Similarity):** - Calculates the cosine of the angle between the Job Description vector and the Resume vector to determine a match percentage.

---

## 🛠️ Technical Stack
- **Language:** Python
- **Libraries:** NLTK, Scikit-Learn, Pandas, Matplotlib, Seaborn
- **Development Environment:** VS Code / Jupyter Notebooks

## 📂 Project Structure
- `src/`: Modular scripts for text cleaning and similarity calculations.
- `notebooks/`: Exploratory Data Analysis and pipeline testing.
- `assets/`: Result charts used for the final report.
- `data/`: Sample resumes and job descriptions (PDF/Text).

## 🚀 Setup & Execution
1. **Clone the Repo:**
   ```bash
   git clone [https://github.com/your-username/AI-Resume-Analyser.git](https://github.com/your-username/AI-Resume-Analyser.git)
