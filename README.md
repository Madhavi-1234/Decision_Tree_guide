# Decision Tree Guide

A simple, step-by-step implementation of a Decision Tree Classifier on the Iris dataset — covering data exploration, model building, visualization, and post-pruning.

## What's Covered

1. **Data Loading** — Loading the Iris dataset from sklearn
2. **Exploratory Data Analysis (EDA)** — Understanding dataset shape, features, and target classes
3. **Train-Test Split** — Splitting data for training and evaluation
4. **Building the Decision Tree** — Training a `DecisionTreeClassifier` using Gini Index / Entropy as splitting criteria
5. **Visualizing the Tree** — Plotting the tree structure to see how splits happen at each node
6. **Model Evaluation** — Checking accuracy and confusion matrix on test data
7. **Post-Pruning (Cost Complexity Pruning)** — Reducing overfitting by pruning the tree using `ccp_alpha`

## Key Concepts Used

- **Entropy / Gini Index** — Measures used to decide the best feature to split on at each node
- **Information Gain** — Used to compare splits and pick the one that reduces impurity the most
- **Overfitting** — A fully grown tree memorizes training data; pruning helps it generalize better
- **Post-Pruning** — After building the full tree, less useful branches are removed using cost complexity pruning (`ccp_alpha`), improving performance on unseen/test data

## How to Run

```bash
pip install scikit-learn matplotlib pandas numpy
```

Open the notebook and run all cells in order. Each section is commented to explain what's happening at every step.

## Dataset

Built-in **Iris dataset** from `sklearn.datasets` — 150 samples, 4 features (sepal/petal length & width), and 3 target classes (Setosa, Versicolor, Virginica).

## Goal

A beginner-friendly reference for understanding how a Decision Tree works internally — from splitting logic (entropy/gini) to controlling overfitting through post-pruning.
