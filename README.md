# 🏎️ F1 Podium Predictor – AI Exam Project

This project is part of my  AI exam (Summer 2025) at Cphbusiness. It includes both supervised and unsupervised learning models, as well as a local AI-powered app using Streamlit to simulate podium finish predictions for Formula 1 races.


## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/f1-ai-exam.git
cd f1-ai-exam
```

### 2. Set up virtual environment
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r part2_app/requirements.txt
```

### 3. Launch the local Streamlit app
```bash
cd part2_app
streamlit run app.py
```

## Data
All CSV files are inside `data/f1Data/`. They come from the Kaggle Formula 1 World Championship dataset.

## Features Used for Prediction
- Grid position
- Driver ID
- Constructor ID
- Race year
- Race round

## Machine Learning Models
**Supervised**: Random Forest Classifier to predict podium finishes (top 3).
**Unsupervised**: KMeans clustering and PCA for driver profiling (e.g. Comeback Driver).

## About the Exam
This project was made for the final AI course exam at Cphbusiness and is split into two parts:
- Part 1: ML pipeline + evaluation
- Part 2: Deployment of a local model using Streamlit

## Credits
- Dataset: https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020
- Student: Vivek Singh Nagra

## Part 1: Machine Learning Notebook

The file `part1_notebook.ipynb` contains the full pipeline of the supervised and unsupervised machine learning work done for this exam.

**Key tasks in Part 1 include:**
- Loading and merging historical F1 race data
- Engineering a `podium_finish` feature (Top 3 result prediction)
- Training a **Random Forest Classifier** to predict podium finishes
- Performing **KMeans Clustering** with PCA to group drivers by performance patterns
- Creating performance profiles such as *Comeback Driver*, *Consistent Midfielder*, etc.

The notebook is fully commented and includes code outputs and explanations of each step.


