# 🏦 Credit Risk Modeling & Scorecard System

For Lauki Finance (NBFC)
📌 Project Overview

This project focuses on the development of an end-to-end Credit Risk Modeling System for Lauki Finance, a Non-Banking Financial Company (NBFC). The goal is to help the business make faster, data-driven, and explainable lending decisions.

The system predicts the probability of loan default and converts that risk into a business-friendly credit scorecard that categorizes applicants into:

Poor | Average | Good | Excellent

This enables both risk reduction and operational efficiency in the loan approval process.

🎯 Business Objective

Traditional credit evaluation processes are often:

Slow

Heavily manual

Inconsistent across decision-makers

This solution helps Lauki Finance:

✔ Assess borrower risk using historical lending data
✔ Standardize decision-making through a scorecard
✔ Reduce defaults by identifying high-risk applicants
✔ Enable Straight Through Processing (STP) for low-risk applications

🧠 Solution Overview

The project delivers a machine learning-powered credit risk engine with a user-facing application for real-time evaluation.

🔹 Core Components

Predictive Credit Risk Model
Estimates the probability of default (PD) using borrower demographics, loan details, and bureau data.

Credit Scorecard System
Converts model output into a simplified, business-friendly risk rating:

Poor – Very high default risk

Average – Moderate risk

Good – Low risk

Excellent – Very low risk

Streamlit Web Application
A UI for loan officers to input applicant details and instantly receive:

Default probability

Credit risk category

Supporting risk drivers

Model Monitoring & ML Ops Framework
Designed to track model performance post-deployment and support production integration.

🏗️ Project Architecture

Data → Feature Engineering → Model → Scorecard → Streamlit App → Monitoring

Historical loan & repayment data used for model training

Feature engineering aligned with real lending behavior

Model predictions translated into interpretable risk categories

Application layer built for business usability

📊 Model Development

The model was trained using Lauki Finance’s historical lending dataset, including:

Borrower demographics

Loan attributes (amount, tenure, type, etc.)

Credit bureau indicators (utilization, open accounts, etc.)

Historical repayment/default behavior

Key Focus Areas

Handling class imbalance in default data

Feature selection based on risk relevance

Model explainability to support business trust

Probability calibration for reliable score mapping

🧮 Credit Scorecard Design

Instead of exposing raw probabilities, the system converts predictions into decision-ready categories.

Risk Category	Interpretation	Business Use
Poor	Very high likelihood of default	Likely rejection or strict review
Average	Moderate risk	Manual underwriting
Good	Low risk	Faster approval
Excellent	Very low risk	Eligible for STP

This bridges the gap between data science outputs and credit policy decisions.

💻 Streamlit Application

A lightweight, user-friendly interface built for loan officers.

Users Can:

Enter applicant and loan details

Provide bureau-related metrics

Instantly receive:

Probability of default

Risk category (Poor–Excellent)

Model-driven assessment

This ensures the model is not just accurate, but usable in daily lending operations.

🔍 Model Monitoring & MLOps (Planned / Phase 2)

To ensure long-term reliability, the system is designed for:

Performance Monitoring
Track model accuracy, stability, and drift over time

Data Drift Detection
Identify shifts in borrower behavior or portfolio profile

Business Rule Integration
Combine model output with lending policies

Straight Through Processing (STP)
Automatically approve high-confidence, low-risk applications

🛠️ Tech Stack

Python – Core modeling and data processing

Pandas / NumPy – Data manipulation

Scikit-learn / ML Libraries – Model development

Streamlit – Front-end application

Matplotlib / Seaborn – Visualization

Joblib / Pickle – Model serialization

📁 Repository Structure (Example)
├── data/                  # Raw and processed datasets
├── notebooks/             # EDA and model development notebooks
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   └── scorecard.py
├── app/
│   └── streamlit_app.py   # Streamlit UI
├── models/                # Saved model files
├── reports/               # Model evaluation reports
└── README.md

▶️ How to Run the Application
# Clone the repository
git clone <your-repo-link>

# Navigate to project folder
cd credit-risk-model

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app/streamlit_app.py

📈 Key Outcomes

✔ Built an explainable credit risk model
✔ Translated model output into a practical business scorecard
✔ Developed a real-time decision-support application
✔ Designed a foundation for production monitoring and STP

⚠️ Disclaimer

This project was developed for educational and portfolio purposes based on a simulated business case. Any resemblance to real financial institutions or proprietary systems is purely illustrative.
