# RecruitAI-Hybrid-Candidate-Ranking
AI-powered candidate ranking engine combining semantic search, feature engineering, and recruiter behavioral signals to intelligently shortlist top talent.
# RecruitAI: Hybrid AI-Powered Candidate Ranking Engine

## Overview

RecruitAI is an AI-powered candidate ranking engine designed to intelligently shortlist the most relevant candidates by combining semantic understanding with structured recruiter signals.

Unlike traditional Applicant Tracking Systems (ATS) that rely heavily on keyword matching, RecruitAI evaluates candidates using a hybrid scoring approach that incorporates:

* Semantic similarity between job descriptions and candidate profiles
* AI career progression
* Technical skill relevance
* Production machine learning experience
* Product company background
* Recruiter behavioral signals
* Penalty mechanisms for keyword inflation and consulting-only profiles

The system produces an explainable, ranked shortlist to support faster and more informed hiring decisions.

---

## Problem Statement

Traditional recruitment systems often overlook qualified candidates because they depend primarily on exact keyword matches.

RecruitAI addresses this challenge by understanding both the context of a candidate's experience and multiple structured hiring signals, enabling more accurate and meaningful candidate ranking.

---

## Key Features

* Semantic candidate-job matching using Sentence Transformers
* Multi-signal feature engineering
* AI-specific career progression analysis
* Production ML experience detection
* Product company experience scoring
* Recruiter behavioral signal integration
* AI keyword inflation penalty
* Explainable recruiter reasoning
* Ranked candidate shortlist generation

---

## System Architecture

```
Job Description
        │
        ▼
Semantic Embedding
        │
        ▼
Candidate Profiles
        │
        ▼
Feature Engineering
 ├── Experience
 ├── AI Career
 ├── AI Skills
 ├── Production Experience
 ├── Product Company Experience
 ├── Recruiter Signals
 ├── Penalties
        │
        ▼
Hybrid Scoring Engine
        │
        ▼
Ranked Candidate Shortlist
```

---

## Methodology

The ranking pipeline consists of four major stages:

### 1. Candidate Feature Engineering

Structured features are extracted from every candidate profile, including:

* Years of experience
* AI skill score
* AI career score
* Production ML experience
* Product company background
* Recruiter behavioral metrics
* Consulting penalty
* AI keyword inflation penalty

---

### 2. Semantic Matching

Candidate profiles and the target job description are converted into dense vector embeddings using the Sentence Transformers model.

Semantic similarity is computed using cosine similarity to measure contextual relevance beyond simple keyword overlap.

---

### 3. Hybrid Candidate Scoring

RecruitAI combines semantic similarity with engineered recruiter signals using a weighted scoring framework.

Major components include:

* Semantic similarity
* AI career relevance
* Technical skill strength
* Experience fit
* Production experience
* Recruiter behavior
* Product company experience
* Penalty adjustments

This hybrid approach balances contextual understanding with structured hiring indicators.

---

### 4. Explainable Ranking

For every candidate, RecruitAI generates recruiter-friendly explanations describing why a candidate ranked highly, such as:

* Strong semantic match
* Production ML experience
* Relevant AI skills
* Product company experience
* Strong recruiter signals
* Ideal experience range

---

## Technologies Used

* Python
* Google Colab
* Sentence Transformers
* NumPy
* Pandas
* Scikit-learn
* FAISS
* Graphviz

---

## Repository Structure

```
RecruitAI/
│
├── RecruitAI.ipynb
├── README.md
├── requirements.txt
├── submission.csv
├── architecture.png
│
├── data/
│   ├── candidate_schema.json
│   ├── job_description.docx
│   └── redrob_signals.docx
│
└── outputs/
    ├── top20_check.csv
    ├── top100_check.csv
    └── features_final.csv
```

---

## How to Run

1. Clone the repository.
2. Install the required dependencies.

```
pip install -r requirements.txt
```

3. Open the notebook in Google Colab.

4. Mount Google Drive.

5. Place the challenge dataset inside the configured project directory.

6. Execute the notebook sequentially.

The notebook generates:

* Candidate features
* Semantic similarity scores
* Hybrid ranking
* Final submission.csv

---

## Output

RecruitAI produces:

* Ranked candidate shortlist
* Recruiter explanations
* Candidate confidence scores
* Submission file in the required competition format

---

## Future Improvements

Potential enhancements include:

* Cross-encoder re-ranking
* Learning-to-Rank (LambdaMART/XGBoost Ranker)
* Dynamic feature weight optimization
* Real-time recruiter feedback loops
* LLM-generated candidate summaries
* Multi-job ranking support

---

## License

This project is released under the MIT License.
