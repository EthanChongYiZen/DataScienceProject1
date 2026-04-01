# Music Genre Recommender

A machine learning project that predicts a user's preferred music genre based on their age and gender, using a Decision Tree classifier.

## Overview

This project uses a small synthetic dataset (`music.csv`) to train a classification model that recommends music genres such as HipHop, Jazz, Classical, Dance, and Acoustic.

## Tech Stack

- Python 3
- pandas
- scikit-learn
- joblib
- Graphviz (for tree visualization)

## Getting Started

**Prerequisites**

```bash
pip install pandas scikit-learn joblib
```

**Run the notebook**

1. Clone the repository
2. Place `music.csv` in the project root
3. Open `DataScienceProject1.ipynb` in Jupyter and run all cells

## Dataset

The dataset contains 18 records with the following columns:

| Column | Description |
|--------|-------------|
| age | Age of the user |
| gender | 1 = Male, 0 = Female |
| genre | Preferred music genre (target) |

## Workflow

1. Load and inspect data
2. Split features (`age`, `gender`) and target (`genre`)
3. Train/test split (80/20)
4. Train a `DecisionTreeClassifier`
5. Evaluate accuracy
6. Persist model using `joblib`
7. Export tree visualization as `.dot` file

## Output Files

- `music-recommender.joblib` — saved trained model
- `music-recommender.dot` — decision tree visualization (open with Graphviz)

## Notes

- The dataset is made up / synthetic, intended for learning purposes
- Model accuracy may vary on each run due to random train/test splitting
