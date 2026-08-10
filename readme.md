# 🤖 Machine Learning Algorithms

> A hands-on repository documenting my journey of learning, understanding, and implementing Machine Learning algorithms.

This repository contains my **Machine Learning algorithm learning and implementation journey**.

The goal is not just to use Machine Learning libraries, but to understand **how each algorithm works internally**, the mathematics behind it, how it learns from data, how it makes predictions, its important hyperparameters, strengths, limitations, and practical behavior.

I update this repository continuously as I learn and implement new algorithms.

---

## 🎯 Goal

The main objective is to understand Machine Learning algorithms from the inside out.

For every algorithm, I aim to understand:

```text
Problem
   ↓
Intuition
   ↓
How the Algorithm Works
   ↓
Mathematical Foundation
   ↓
Training Process
   ↓
Prediction Process
   ↓
Hyperparameters
   ↓
Model Behavior
   ↓
Overfitting / Underfitting
   ↓
Experiments
   ↓
Practical Applications
```

I don't want to stop at:

```python
model.fit(X_train, y_train)
```

I want to understand:

> **What actually happens when `model.fit()` runs?**

---

# 📚 Algorithms

## Supervised Learning

### Regression

* [x] Linear Regression
* [x] Multiple Linear Regression
* [x] Polynomial Regression
* [x] Ridge Regression
* [x] Lasso Regression
* [x] Elastic Net
* [x] Decision Tree Regression

### Classification

* [x] Logistic Regression
* [x] K-Nearest Neighbors (KNN)
* [x] Naive Bayes
* [x] Support Vector Machine (SVM)
* [x] **Decision Tree** 🌳
* [ ] Random Forest
* [ ] AdaBoost
* [ ] Gradient Boosting
* [ ] XGBoost

> **Note:** The algorithms marked as completed represent the concepts I have already studied and implemented up to my current learning stage.

---

# 🌳 Current Completed Stage — Decision Tree

**Decision Tree is the latest completed algorithm in this repository.**

I have been studying the algorithms progressively, and my current learning has reached **Decision Trees**.

The focus has been on understanding the algorithm beyond simply using `scikit-learn`.

### Decision Tree Concepts

* Tree structure
* Root node
* Internal nodes
* Leaf nodes
* Splitting
* Recursive partitioning
* Decision boundaries
* Feature selection
* Threshold selection
* Stopping criteria

### Splitting Criteria

* Gini Impurity
* Entropy
* Information Gain

### Model Behavior

* Pure and impure nodes
* Tree depth
* Recursive splitting
* Overfitting
* Underfitting
* Model complexity
* Feature importance

### Important Hyperparameters

```python
DecisionTreeClassifier(
    criterion="gini",
    splitter="best",
    max_depth=None,
    min_samples_split=2,
    min_samples_leaf=1,
    max_features=None,
    max_leaf_nodes=None,
    min_impurity_decrease=0.0,
    class_weight=None,
    random_state=None
)
```

I experiment with these parameters to understand how they affect:

* Tree structure
* Model complexity
* Training performance
* Generalization
* Overfitting

### Questions I Try to Answer

Instead of only asking:

> How do I train a Decision Tree?

I try to understand:

* Why was this feature selected?
* Why was this threshold selected?
* How is impurity calculated?
* How is information gain calculated?
* How does the tree decide when to stop splitting?
* Why does a Decision Tree overfit?
* How does `max_depth` affect the model?
* How do other hyperparameters control complexity?
* How does the trained tree make a prediction?

---

# 🔬 How I Study Each Algorithm

For each Machine Learning algorithm, I follow a learning process like:

### 1. Understand the Problem

What type of problem does the algorithm solve?

```text
Classification
Regression
Clustering
Dimensionality Reduction
```

### 2. Understand the Intuition

First understand the idea behind the algorithm without depending on code.

### 3. Understand the Mathematics

Study the mathematical concepts required to understand why the algorithm works.

### 4. Understand Training

How does the model learn from the training data?

### 5. Understand Prediction

How does the trained model produce an output?

### 6. Implement

Implement the algorithm using Python and, where practical, from scratch.

### 7. Use Scikit-Learn

Implement the same algorithm using the standard Machine Learning library.

### 8. Experiment

Change hyperparameters and observe what happens.

### 9. Analyze

Study:

* Model performance
* Model complexity
* Overfitting
* Underfitting
* Training behavior
* Prediction behavior

### 10. Compare

Understand how the algorithm differs from other Machine Learning algorithms.

---

# 🧪 Experimentation

An important part of this repository is **experimentation**.

I don't want to simply run an algorithm once and record the accuracy.

Instead:

```text
Change Parameter
       ↓
Train Model
       ↓
Observe Model
       ↓
Evaluate
       ↓
Visualize
       ↓
Understand Why It Changed
```

For example:

```text
max_depth = 2
      ↓
Simple Tree
      ↓
Possible Underfitting
```

compared with:

```text
max_depth = 20
      ↓
Complex Tree
      ↓
Possible Overfitting
```

This helps me understand the relationship between:

```text
Data
 +
Algorithm
 +
Hyperparameters
        ↓
Model Behavior
        ↓
Performance
```

---

# 🧠 Concepts I Track Across Algorithms

As I progress through different algorithms, I continuously study concepts that appear across multiple models.

### Model Complexity

How the complexity of a model affects its ability to learn.

### Bias-Variance Tradeoff

Understanding:

* Bias
* Variance
* Underfitting
* Overfitting
* Generalization

### Hyperparameters

Understanding:

* What each parameter controls
* Why it exists
* What happens when it increases
* What happens when it decreases

### Optimization

Understanding how algorithms find their parameters or solutions.

### Decision Boundaries

Understanding how classification algorithms separate different classes.

### Feature Importance

Understanding how different algorithms determine which features are useful.

---

# 📁 Repository Structure

```text
machine-learning-algorithms/
│
├── README.md
│
├── supervised_learning/
│   │
│   ├── regression/
│   │   ├── linear_regression/
│   │   ├── polynomial_regression/
│   │   ├── ridge/
│   │   ├── lasso/
│   │   └── decision_tree/
│   │
│   └── classification/
│       ├── logistic_regression/
│       ├── knn/
│       ├── naive_bayes/
│       ├── svm/
│       ├── decision_tree/
│       ├── random_forest/
│       └── gradient_boosting/
│
├── unsupervised_learning/
│   │
│   ├── clustering/
│   │   ├── kmeans/
│   │   ├── hierarchical/
│   │   └── dbscan/
│   │
│   └── dimensionality_reduction/
│       └── pca/
│
└── experiments/
```

The structure will evolve as I continue learning.

---

# 📊 Learning Progress

|  # | Algorithm                  | Type                     | Status                    |
| -: | -------------------------- | ------------------------ | ------------------------- |
|  1 | Linear Regression          | Regression               | ✅ Completed               |
|  2 | Multiple Linear Regression | Regression               | ✅ Completed               |
|  3 | Polynomial Regression      | Regression               | ✅ Completed               |
|  4 | Ridge Regression           | Regression               | ✅ Completed               |
|  5 | Lasso Regression           | Regression               | ✅ Completed               |
|  6 | Elastic Net                | Regression               | ✅ Completed               |
|  7 | Logistic Regression        | Classification           | ✅ Completed               |
|  8 | KNN                        | Classification           | ✅ Completed               |
|  9 | Naive Bayes                | Classification           | ✅ Completed               |
| 10 | SVM                        | Classification           | ✅ Completed               |
| 11 | **Decision Tree**          | **Classification**       | **✅ Completed — Current** |
| 12 | Random Forest              | Classification           | 🔵 Next                   |
| 13 | AdaBoost                   | Ensemble                 | 🔵 Upcoming               |
| 14 | Gradient Boosting          | Ensemble                 | 🔵 Upcoming               |
| 15 | XGBoost                    | Ensemble                 | 🔵 Upcoming               |
| 16 | K-Means                    | Clustering               | 🔵 Upcoming               |
| 17 | Hierarchical Clustering    | Clustering               | 🔵 Upcoming               |
| 18 | DBSCAN                     | Clustering               | 🔵 Upcoming               |
| 19 | PCA                        | Dimensionality Reduction | 🔵 Upcoming               |

---

# 🛠️ Tools

The main tools used for implementations and experiments:

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-Learn**
* **Jupyter Notebook**
* **VS Code**
* **Git & GitHub**

---

# 📈 Current Learning Position

```text
Machine Learning Algorithms
          │
          ▼
   Supervised Learning
          │
     ┌────┴────┐
     ▼         ▼
Regression  Classification
     │         │
     ▼         ▼
  Learning   Learning
     │         │
     └────┬────┘
          ▼
    🌳 Decision Tree
          │
          ▼
    ✅ Completed
          │
          ▼
   🔵 Random Forest
          │
          ▼
   🔵 Ensemble Learning
          │
          ▼
   🔵 Unsupervised Learning
```

---

# 🚀 Next Step

The next stage after Decision Tree is to continue with:

```text
Decision Tree
      ↓
Random Forest
      ↓
Ensemble Learning
      ↓
Gradient Boosting
      ↓
XGBoost
      ↓
Unsupervised Learning
```

The exact order may change as I continue learning and experimenting.

---

# ⭐ Learning Philosophy

This repository is not intended to be a collection of copied Machine Learning implementations.

Every algorithm should represent actual understanding.

My approach:

```text
📖 Learn
   ↓
🧠 Understand
   ↓
📐 Study the Mathematics
   ↓
💻 Implement
   ↓
🧪 Experiment
   ↓
📊 Analyze
   ↓
🔍 Understand Limitations
   ↓
🚀 Move to the Next Algorithm
```

> **Don't just learn how to use the model. Learn why the model works.**

---

## 🔄 Continuously Updated

This repository is a work in progress.

As I learn new Machine Learning algorithms, I will add their:

* Concepts
* Mathematical intuition
* Implementations
* From-scratch implementations
* Hyperparameters
* Experiments
* Visualizations
* Strengths and weaknesses
* Practical observations

**Current progress: Decision Tree ✅**

**Next: Random Forest 🔵**
