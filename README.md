# Group1-PROG8431-ProblemAnalysis_Workshop_A
Problem Analysis Workshop A - Repo for submission

# PROG8431 - Problem Analysis Workshop A
**Data Analysis, Mathematics, Modeling and Algorithms**  
**Term Project Exploratory & Statistical Analysis**

---

## 📌 Project Overview
This project performs an exploratory data analysis and inferential statistical evaluation on the **AI4I 2020 Predictive Maintenance Dataset** sourced from the UCI Machine Learning Repository. 

The objective is to:
1. Examine the distributional properties of core operational and sensor metrics.
2. Formally assess normality on key physical stress parameters (`Torque`) using visual Q-Q diagnostics and the Shapiro-Wilk test.
3. Conduct hypothesis testing (Two-sample F-Test for equal variance and Welch's t-test for difference in means) to evaluate whether machinery operating states differ significantly between normal operations and failure modes.

---

## 📂 Repository Structure
```text
├── data/
│   ├── predictive_maintenance.csv             # Extracted predictive maintenance dataset
│   └── predictive_maintenance.zip             # Downloaded archive (ignored in Git)
├── Problem_Analysis_Workshop_A.ipynb          # Main deliverable Jupyter Notebook
├── .gitignore                                 # Ignores archives, checkpoints, and bytecode
└── README.md                                  # Project documentation

---

## 📊 Dataset Information
Source: UCI Machine Learning Repository - AI4I 2020 Predictive Maintenance Dataset

Observations: 10,000 synthetic operational cycles reflecting real milling machine parameters.

Key Features Examined:
air_temp [K]: Ambient factory temperature.
process_temp [K]: Machining process temperature.
rotational_speed [rpm]: Spindle rotation speed.
torque [Nm]: Mechanical resistance / load.
tool_wear [min]: Cumulative cutting tool wear duration.
machine_failure [0/1]: Binary target variable indicating failure state.

---

## Setup and configuration
Clone the repository using the above link:
```bash
git clone https://github.com/DavisenV/Group1-PROG8431-ProblemAnalysis_Workshop_A.git
```
Open a terminal and navigate to the root directory
```bash
cd ./"your path here"
```
Create a virtual environment and activate
```bash
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```
Install all the required using the requirements.txt
```bash
python -m pip install -r requirements.txt
```