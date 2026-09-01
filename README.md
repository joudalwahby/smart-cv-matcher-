# 📄 Smart CV & Job Matcher System (NLP Driven)

An end-to-end NLP application built to parse, process, and evaluate the degree of match between a candidate's Resume (PDF) and a specific Job Description (JD).

This tool is designed to mimic Automated Resume Screening / Applicant Tracking Systems (ATS) to provide actionable feedback on candidate-job keyword alignment.

> **Note:** Run the application locally following the setup steps below.

---

## ✨ Features

* **PDF Text Extraction:** Parses text directly from uploaded PDF resumes using `pypdf`.
* **Keyword Matching & Vectorization:** Transforms unstructured text into numerical representations using **TF-IDF (Term Frequency-Inverse Document Frequency)** vectorization.
* **Similarity Scoring:** Calculates a precise match score percentage using **Cosine Similarity**.
* **Visual & Quantitative Feedback:** Provides instant progress visualizers and targeted recommendations (High / Moderate / Low Alignment).

---

## 🛠️ Tech Stack & Libraries

* **Language:** Python 3.10+
* **Framework:** Streamlit (UI & Web Deployment)
* **NLP & ML:** Scikit-Learn (`TfidfVectorizer`, `cosine_similarity`)
* **File Parsing:** PyPDF

---

## 💻 How It Works

1. **Extraction:** The user uploads a PDF resume and pastes a Job Description.
2. **Preprocessing:** Text is extracted, cleaned, and stripped of common English stop words.
3. **Vectorization:** Sentences are mapped into a high-dimensional vector space using TF-IDF.
4. **Scoring:** Cosine Similarity measures the angular distance between the CV vector and JD vector to output a percentage match.

---

## 🛠️ Local Installation & Setup

If you wish to run this project locally:

```bash
# 1. Clone the repository
git clone [https://github.com/joudalwahby/smart-cv-matcher.git](https://github.com/joudalwahby/smart-cv-matcher.git)

# 2. Change directory
cd smart-cv-matcher

# 3. Install requirements
pip install -r requirements.txt

# 4. Run the Streamlit app
streamlit run app.py
