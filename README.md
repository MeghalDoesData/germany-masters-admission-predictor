# Germany Master's Admission Predictor 🇩🇪

An exploratory data analytics and machine learning project to investigate and estimate admission outcomes for Master's programmes in Germany.

The project aims to collect applicant profiles and application outcomes, identify factors associated with admission decisions, and eventually build a model that estimates the probability of admission for a given applicant–programme combination.

> **Status:** 🚧 Early stage — Data Collection

---

## 🎯 Objective

Every year, applicants to German universities ask questions like:

> *"With my CGPA, IELTS score, internships, and work experience, what are my chances of getting admitted?"*

There is plenty of anecdotal information available online, but relatively little structured applicant-level data.

This project aims to turn those experiences into a structured dataset and explore:

* Which applicant characteristics are associated with admission?
* Which factors appear to matter most?
* How do outcomes differ between programmes and universities?
* Can machine learning provide a useful estimate of admission probability?
* How reliable and well-calibrated are those predictions?

The eventual goal is **not to replace university admission decisions**, but to build an analytical model based on historical applicant data.

---

## 🧩 Project Approach

The project will follow an end-to-end data analytics workflow:

```text
Applicant Survey
       │
       ▼
Raw Applicant Data
       │
       ▼
Data Cleaning & Validation
       │
       ▼
Exploratory Data Analysis
       │
       ▼
Feature Engineering
       │
       ▼
Statistical Analysis
       │
       ▼
Machine Learning Models
       │
       ▼
Model Evaluation & Calibration
       │
       ▼
Admission Probability
       │
       ▼
Interactive Application
```

---

## 📊 Data

The initial dataset will be collected through a voluntary survey of applicants who have applied to Master's programmes in Germany.

Potential variables include:

### Applicant Profile

* Bachelor's degree
* Bachelor's field
* CGPA / percentage
* Degree duration
* Country of application
* Graduation year

### Test Scores

* IELTS / TOEFL
* GRE / GMAT

### Experience

* Work experience
* Internships
* Research experience
* Publications

### Application

* University
* Master's programme
* Intake
* Application route
* Whether stated admission requirements were met

### Outcome

* Admitted
* Rejected
* Waitlisted
* Pending
* Withdrawn

If an applicant applies to multiple universities, applications may be recorded separately so that each **applicant–programme application** represents an observation.

---

## 🤖 Planned Machine Learning

The project will experiment with several approaches rather than relying on a single model.

Potential models include:

* Logistic Regression
* Decision Tree
* Random Forest
* Gradient Boosting / XGBoost

Model performance will be evaluated using appropriate classification metrics such as:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC
* Precision-Recall
* Probability calibration

Where appropriate, model interpretability techniques such as feature importance and SHAP will be explored.

---

## 📈 Planned Analysis

Some of the questions we hope to investigate:

* How does CGPA relate to admission outcomes?
* Does work experience appear to influence outcomes?
* Does research experience provide an advantage?
* How important are English-language test scores?
* How do outcomes vary between programmes?
* How much does the university/programme itself influence predictions?
* Are there meaningful differences between applicant profiles across intakes?

---

## 🛠️ Planned Tech Stack

The exact stack may evolve as the project develops.

**Data & Analysis**

* Python
* Pandas
* NumPy
* Jupyter
* Matplotlib / Seaborn

**Machine Learning**

* Scikit-learn
* XGBoost
* SHAP

**Application**

* Streamlit

**Development**

* Git
* GitHub

---

## 📁 Project Structure

The repository will gradually evolve into something similar to:

```text
germany-masters-admission-predictor/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   └── 04_modeling.ipynb
│
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   └── evaluation/
│
├── app/
│
├── reports/
│
├── requirements.txt
├── README.md
└── LICENSE
```

This structure is intentionally expected to change as the project develops.

---

## ⚠️ Limitations

This project will have several important limitations.

The dataset is based primarily on voluntary, self-reported applicant information. This can introduce:

* Selection bias
* Self-reporting bias
* Uneven representation across universities and programmes
* Small sample sizes for individual programmes
* Differences in admission criteria between universities
* Changes in admission policies between intakes

Therefore, model predictions should be interpreted as **estimates based on observed historical data**, not as official admission probabilities.

A major part of the project will be understanding these limitations rather than hiding them.

---

## 🔒 Privacy

No personally identifying information is required for the survey.

The project will avoid collecting information such as:

* Names
* Email addresses
* Application IDs
* Passport information
* Phone numbers
* Other sensitive personal identifiers

Only information relevant to the analytical objective should be collected.

---

## 🚧 Current Status

### Phase 1 — Data Collection

* [ ] Design survey
* [ ] Publish survey
* [ ] Collect initial responses
* [ ] Define dataset schema
* [ ] Establish data dictionary

### Phase 2 — Data Preparation

* [ ] Clean data
* [ ] Handle missing values
* [ ] Detect inconsistent responses
* [ ] Encode categorical variables
* [ ] Create analytical dataset

### Phase 3 — Analysis

* [ ] Exploratory Data Analysis
* [ ] Statistical analysis
* [ ] Feature engineering
* [ ] Identify important variables

### Phase 4 — Machine Learning

* [ ] Establish baseline model
* [ ] Train classification models
* [ ] Compare models
* [ ] Evaluate probability calibration
* [ ] Interpret predictions

### Phase 5 — Application

* [ ] Build admission probability estimator
* [ ] Create interactive interface
* [ ] Deploy application
* [ ] Document findings

---

## 📜 Disclaimer

This is an independent analytics project and is **not affiliated with DAAD, Uni-Assist, or any German university**.

The predictions generated by this project should not be considered official admission decisions or guarantees of admission.

---

## 👤 Project

Built as a personal data analytics and machine learning project.

The project is being developed incrementally, starting with data collection and gradually progressing toward statistical analysis, machine learning, and deployment.
