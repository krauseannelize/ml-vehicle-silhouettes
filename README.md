# Vehicle Silhouettes Machine Learning

Supervised and unsupervised machine learning models classifying vehicle silhouettes from geometric features, using Python (scikit-learn, Pandas, NumPy).

## Tools & Skills Used

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat&logoColor=white)
![uv](https://img.shields.io/badge/uv-DE5FE9?style=flat&logo=uv&logoColor=white)

## Quick Access

- [Project Description](project-description.md)
- [Supervised Learning Notebook](notebooks/01-supervised.ipynb)
- [Unsupervised Learning Notebook](notebooks/02-unsupervised.ipynb)
- [Vehicle Silhouettes Dataset](data/vehicle-silhouettes.csv)
- [Cleaned Dataset](data/vehicle-silhouettes-clean.csv)

## Setup & Installation

### Prerequisites

- Python 3.12+
- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager

### 1. Clone the Repository

```bash
git clone https://github.com/krauseannelize/ml-vehicle-silhouettes.git
cd ml-vehicle-silhouettes
```

### 2. Install Dependencies

```bash
uv sync
```

### 3. Run the Project

```bash
uv run jupyter lab
```

📌 **Note:** `uv run` automatically uses the project's virtual environment, no manual activation needed

## Project Overview

**Prospect Auto**, a chain of car repair shops, requested models to classify vehicles based on silhouette features. This repo demonstrates two approaches:

- **Supervised classification** → Predicting vehicle classes using labeled data.
- **Unsupervised clustering** → Grouping vehicles without labels to discover natural structure.

## Objectives

- Explore the Vehicle Silhouettes dataset.
- Build supervised models to classify vehicles.
- Apply unsupervised clustering methods to group vehicles.
- Compare results and assess which approach is most effective.

## Methodology

1. **Data Preparation**

   - Load and clean dataset.
   - Normalize and standardize features.
   - Split into training/testing subsets.

2. **Supervised Learning**

   - Train classification models.
   - Evaluate with accuracy, precision, recall, F1‑score.

3. **Unsupervised Learning**

   - Apply PCA for dimensionality reduction.
   - Train clustering models (e.g., k‑means).
   - Evaluate with silhouette score and inertia.

## Key Findings

- All supervised algorithms performed consistently well across classes, confirming strong generalization without significant overfitting.
- Logistic Regression emerged as the most balanced and reliable supervised model, achieving 95.1% accuracy on training data and 93.9% on test data.
- Unsupervised clustering (K-Means, Hierarchical, DBSCAN) revealed one dominant group with smaller overlapping sub-clusters that were imbalanced and did not align with true vehicle classes.
- While clustering is not a viable alternative for Prospect Auto's classification needs, it may still provide value for exploratory analysis or anomaly detection.
