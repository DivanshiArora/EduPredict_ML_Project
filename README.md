# EduPredict — Student Academic Performance Prediction

## What this project does
EduPredict is a beginner-friendly machine-learning web application. It trains a Linear Regression model on the UCI Student Performance dataset and estimates a student's final grade (G3) from:
- Weekly study-time category (`studytime`)
- Past class failures (`failures`)
- Absences (`absences`)
- First-period grade (`G1`)
- Second-period grade (`G2`)

It also displays dataset charts and model evaluation metrics.

## Requirements
- Python 3.10 or newer recommended
- Internet connection for the first dataset download

## Setup (Windows / VS Code terminal)

```powershell
python -m venv .venv
.venv\Scripts\activate
python -m pip install --upgrade pip
pip install -r requirements.txt
streamlit run app.py
```

A browser tab should open with the application.

## Dataset
UCI Machine Learning Repository, Student Performance dataset:
https://uci-ics-mlr-prod.aws.uci.edu/dataset/320/student%2Bperformance

Citation:
Cortez, P. (2008). Student Performance [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5TG7T.

## Important limitation
This is an educational demonstration using historical data. The previous-period grades G1 and G2 are strongly related to the final grade G3, so the model is most appropriately understood as an estimate made after the first two grading periods—not as a long-term prediction made at the start of a school year. Predictions are not guarantees.

## Main files
- `app.py` — complete Streamlit application
- `requirements.txt` — Python libraries required
