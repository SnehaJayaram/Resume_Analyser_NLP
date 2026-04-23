# 📄 AI Resume Analyser & Ranker (NLP)

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![NLP](https://img.shields.io/badge/Focus-Natural%20Language%20Processing-blueviolet.svg)](#)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)](https://scikit-learn.org/)

## 🎯 The "Sales Pitch": Why This Matters
Traditional recruitment is broken. HR managers spend an average of **6 seconds** looking at a resume before deciding. This project automates that initial screening using **Data Science**, ensuring that the most qualified candidates are never missed due to human fatigue.

By leveraging **Vector Space Modeling**, this tool mathematically calculates the "distance" between a candidate's skills and a company's requirements, providing a transparent, data-driven ranking system.

---

## 📊 Visual Proof of Logic
### 1. Candidate Similarity Ranking
![Similarity Scores](./assets/similarity_score_chart.png)
*How well does each candidate align with the Job Description? Our Cosine Similarity engine provides a definitive match percentage.*

### 2. Automated Skill Distribution
![Skill Distribution](./assets/skill_distribution.png)
*A macro-view of the talent pool, showing which technical skills are most prevalent across all applicants.*

---

## 🧠 Technical Workflow
This system follows a professional NLP pipeline:
1. **Text Extraction:** Using `PyPDF2` to handle unstructured PDF data.
2. **Preprocessing:** Custom scripts for tokenization, removing "noise" (stopwords), and text normalization.
3. **Vectorization (TF-IDF):** Converting words into numerical weights. This ensures that unique technical skills (e.g., "Kubernetes") are weighted more heavily than common words.
4. **Scoring Engine:** Applying **Cosine Similarity** to rank resumes based on their vector proximity to the Job Description.

## 📂 Project Structure
- `src/`: Modular Python scripts for reusable NLP functions.
- `notebooks/`: Full development lifecycle and experimentation.
- `data/`: Sample resumes and JDs used for benchmarking.
- `assets/`: High-resolution visual evidence of system performance.

## 🚀 Quick Start
```bash
# 1. Clone the repository
git clone [https://github.com/your-username/AI-Resume-Analyser.git](https://github.com/your-username/AI-Resume-Analyser.git)

# 2. Install requirements
pip install -r requirements.txt

# 3. View Results
# Run the Jupyter Notebook in the /notebooks folder
