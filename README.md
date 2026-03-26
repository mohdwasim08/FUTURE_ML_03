[README.md](https://github.com/user-attachments/files/26282444/README.md)
#  Resume / Candidate Screening System
### Future Interns – Machine Learning Track | Task 3

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-NLP-green?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

##  Overview

This project is an **ML-powered Resume Screening System** that automatically ranks candidates based on how well their resumes match a given job description. It uses **NLP techniques** (TF-IDF + Cosine Similarity) to score, rank, and identify skill gaps for each candidate.

Built as part of the **Future Interns Machine Learning Internship – Task 3**.

---

##  Objectives

- Parse and clean resume text using NLP
- Match resumes against a job description using TF-IDF vectorization
- Rank candidates by similarity score
- Assign priority labels (High / Medium / Low)
- Identify skill gaps and missing required skills
- Visualize results in a business-ready dashboard

---

##  Project Structure

```
FUTURE_ML_03/
│
├── FUTURE_ML_03.ipynb       # Main Jupyter Notebook (complete project)
├── screening_dashboard.png  # Output dashboard (auto-generated)
└── README.md                # Project documentation
```

---

##  Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.8+ | Core programming language |
| NLTK | Text preprocessing, tokenization, lemmatization |
| Scikit-learn | TF-IDF Vectorizer, Cosine Similarity |
| Pandas | Data manipulation and structuring |
| Matplotlib | Bar charts, pie charts |
| Seaborn | Skill coverage heatmap |

---

##  How It Works

```
Resume Text
    │
    ▼
Text Cleaning (lowercase, remove URLs, punctuation, stopwords, lemmatize)
    │
    ▼
TF-IDF Vectorization (resumes + job description)
    │
    ▼
Cosine Similarity Score (each resume vs JD)
    │
    ▼
Candidate Ranking + Priority Tagging
    │
    ▼
Skill Gap Analysis + Visual Dashboard
```

---

##  Key Features

- **Resume Parsing** — Cleans and normalizes raw resume text
- **JD Matching** — Scores each resume against the job description using TF-IDF + Cosine Similarity
- **Candidate Ranking** — Sorts candidates from best to least fit
- **Priority Tagging** — Labels candidates as High /  Medium / Low
- **Skill Gap Report** — Highlights which required skills are present or missing per candidate
- **4-Panel Dashboard** — Match scores, skill heatmap, priority pie chart, skills comparison bar chart

---

##  Sample Output

```
═══════════════════════════════════════════════════════════════
       FINAL CANDIDATE SCREENING REPORT
      Role: Machine Learning Engineer / Data Scientist
═══════════════════════════════════════════════════════════════
Rank  Candidate       Match %   Priority
1     Sneha Patel      67.4%     High
2     Priya Sharma     58.2%     High
3     Mohd Wasim       34.1%     Medium
4     Rahul Gupta      21.5%     Low
5     Arjun Mehta       8.3%     Low
```

---

##  Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/mohdwasim08/FUTURE_ML_03.git
cd FUTURE_ML_03
```

### 2. Install Dependencies
```bash
pip install nltk scikit-learn pandas numpy matplotlib seaborn jupyter
```

### 3. Run the Notebook
```bash
jupyter notebook FUTURE_ML_03.ipynb
```

> Run all cells top to bottom. NLTK data is auto-downloaded on first run.

---

##  Customization

To screen for a **different job role**, simply edit the `job_description` variable in **Step 4** of the notebook:

```python
job_description = """
We are looking for a [Your Role Here].
Required Skills: [skill1, skill2, ...]
...
"""
```

To add **more resumes**, append to the `resumes` list in **Step 2**:

```python
resumes.append({
    "name": "Candidate Name",
    "text": "Resume text here..."
})
```

---

##  Skills Gained

- Natural Language Processing (NLP)
- Text preprocessing and feature extraction
- TF-IDF vectorization
- Cosine similarity for document matching
- Resume scoring and ranking models
- Data visualization with Matplotlib & Seaborn

---

## Author

**Mohammad Wasim**
-  mohdwasim.tech@gmail.com
-  [github.com/mohdwasim08](https://github.com/mohdwasim08)
-  B.Tech Mechanical Engineering, Zakir Husain College of Engineering and Technology

---

##  Internship Details

| Field | Details |
|-------|---------|
| Organization | Future Interns |
| Domain | Machine Learning |
| Task | Task 3 – Resume / Candidate Screening System |
| Repository Format | `FUTURE_ML_03` |
| Website | [futureinterns.com](https://futureinterns.com) |

---

## License

This project is submitted as part of the Future Interns ML Internship program. Free to use for educational purposes.
