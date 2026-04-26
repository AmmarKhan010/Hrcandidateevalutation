# HR Candidate Screening Assistant

### AI-Powered CV Matching for Intelligent Recruitment

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python\&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-TF--IDF%20%7C%20Similarity-6A0DAD)
![Machine Learning](https://img.shields.io/badge/ML-Text%20Matching-FF6F00)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-FF4B4B?logo=streamlit\&logoColor=white)
![Cloud](https://img.shields.io/badge/Cloud-Colab%20%7C%20ngrok-1E90FF)
![Status](https://img.shields.io/badge/Status-Prototype-FF8C00)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## Overview

The **HR Candidate Screening Assistant** is a lightweight AI-powered web application designed to **streamline the initial recruitment process**.

It leverages **Natural Language Processing (NLP)** techniques to evaluate how well a candidate’s CV aligns with a given job description, enabling **faster, data-driven hiring decisions**.

This tool demonstrates how **AI can augment HR workflows** by reducing manual screening effort and improving consistency in candidate evaluation.

---

## Key Features

* **Custom Job Criteria Input**
  Define required skills, experience, and qualifications dynamically via the sidebar

* **Automated CV Analysis**
  Upload and evaluate candidate CVs in `.txt` format

* **AI-Based Matching Engine**
  Uses TF-IDF vectorization and cosine similarity to compute relevance scores

* **Quantitative Match Score**
  Generates a percentage-based similarity score for objective comparison

* **Interview Recommendation System**
  Provides automated suggestions based on match thresholds

* **Cloud Deployment Ready**
  Easily deployable using Google Colab and ngrok for quick prototyping

---

## System Architecture

**Input Layer**

* Job description / required attributes
* Candidate CV (text format)

**Processing Layer**

* Text preprocessing
* Feature extraction using TF-IDF
* Similarity computation using cosine similarity

**Output Layer**

* Match percentage score
* Interview recommendation

---

## How It Works

The application applies a **vector-space model** to compare textual data:

### 1. TF-IDF (Term Frequency – Inverse Document Frequency)

Transforms text into weighted numerical vectors based on word importance.

### 2. Cosine Similarity

Measures similarity between job description and CV vectors by calculating the angle between them.

**Result:**
A score between **0 and 1 (or 0%–100%)** representing candidate relevance.

---

## Project Structure

hr-screening-assistant/

├── app.py              # Main Streamlit application
├── requirements.txt    # Dependencies
├── notebooks/
│   └── colab_run.ipynb # Colab setup with ngrok
├── data/
│   └── sample_cv.txt   # Sample CV
└── README.md           # Documentation

---

## Installation

```bash
git clone https://github.com/your-username/hr-screening-assistant.git
cd hr-screening-assistant
pip install -r requirements.txt
```

---

## Running the Application (Local)

```bash
streamlit run app.py
```

---

## Running on Google Colab

1. Open the provided notebook (`colab_run.ipynb`)
2. Install dependencies (`streamlit`, `pyngrok`)
3. Add your **ngrok auth token**
4. Launch the app
5. Access via generated public URL

---

## Usage

1. **Define Job Requirements**
   Enter keywords such as:

   * Python
   * Data Analysis
   * Project Management

2. **Upload Candidate CV**
   Upload a `.txt` file

3. **Review Results**

   * Match Score (%)
   * Interview Recommendation

---

## Example Output

Match Score: **82%**
Recommendation: **Proceed to Interview**

---

## Limitations

* Supports **.txt files only**
* Basic keyword-based semantic matching
* Does not capture deep contextual meaning or soft skills

---

## Future Enhancements

* PDF and DOCX support (PyPDF2, python-docx)
* Transformer-based NLP models (e.g., BERT embeddings)
* Multi-candidate ranking system
* Bias detection and fairness evaluation
* Integration with ATS (Applicant Tracking Systems)
* Explainable AI for transparent decision-making

---

## Applications

This system can be extended for:

* Automated HR screening pipelines
* Talent acquisition platforms
* Enterprise recruitment systems
* AI-assisted decision support tools

---

## Author

**Ammar Akhter Khan**
AI Researcher | Intelligent Systems | Applied Machine Learning

---

## License

Distributed under the MIT License
© 2026 Ammar Akhter Khan
