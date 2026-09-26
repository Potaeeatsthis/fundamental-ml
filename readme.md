# 2026 KMITL Data Analytics

A Google Colab course that teaches Python data tools, data preparation, machine
learning, and deep learning.

## Purpose

Each notebook is a complete lesson. Every notebook explains each important
concept in simple words, shows a small numerical example before a large example,
runs real code with no unfinished placeholders, includes at least one chart, and
ends with a short summary of the main ideas.

## Current status

- **Parts 1 to 7 are ready** in the `notebooks/` folder.
- **Parts 8 to 14 are planned** and are not in this repository yet.

The course has 14 parts. It does not include exercises, a final-project part,
a separate large-language-model part, or Part 15.

### Ready parts

| Part | Notebook | Main topics |
|---|---|---|
| 1: Python Tools for Machine Learning | `notebooks/part_01_python_tools.ipynb` | NumPy, pandas, Matplotlib, Seaborn, SciPy, a scikit-learn pipeline |
| 2: Data Preparation | `notebooks/part_02_data_preparation.ipynb` | Cleaning, missing values, duplicates, outliers, scaling, data splits |
| 3: Regression | `notebooks/part_03_regression.ipynb` | Linear and multiple regression, error metrics, gradient descent, polynomials |
| 4: Classification | `notebooks/part_04_classification.ipynb` | KNN, decision trees, logistic regression, support vector machines |
| 5: Model Evaluation and Improvement | `notebooks/part_05_model_evaluation.ipynb` | Confusion matrix, precision and recall, cross-validation, tuning, regularization |
| 6: Clustering | `notebooks/part_06_clustering.ipynb` | Distances, K-means, elbow and silhouette, hierarchical linkage, DBSCAN |
| 7: Recommender Systems | `notebooks/part_07_recommender_systems.ipynb` | Content-based, user- and item-based filtering, matrix factorization, evaluation, cold start |

### Planned parts

| Part | Notebook |
|---|---|
| 8: Neural Network Foundations | `notebooks/part_08_neural_network_foundations.ipynb` |
| 9: Deep Learning with Keras | `notebooks/part_09_deep_learning_with_keras.ipynb` |
| 10: Convolutional Neural Networks | `notebooks/part_10_convolutional_neural_networks.ipynb` |
| 11: Sequence Models | `notebooks/part_11_sequence_models.ipynb` |
| 12: Transformers | `notebooks/part_12_transformers.ipynb` |
| 13: Unsupervised and Generative Deep Learning | `notebooks/part_13_generative_deep_learning.ipynb` |
| 14: Efficient Deep-Learning Training | `notebooks/part_14_efficient_deep_learning.ipynb` |

## Directory structure

```text
2026-kmitl-data-analytics/
├── readme.md
├── requirements.txt
├── data/
│   └── readme.md
└── notebooks/
    ├── part_01_python_tools.ipynb
    ├── part_02_data_preparation.ipynb
    ├── part_03_regression.ipynb
    ├── part_04_classification.ipynb
    ├── part_05_model_evaluation.ipynb
    ├── part_06_clustering.ipynb
    └── part_07_recommender_systems.ipynb
```

## Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Choose **File > Upload notebook** and upload any notebook from the
   `notebooks/` folder.
3. Choose **Runtime > Change runtime type**, select **CPU**, and click **Save**.
4. Choose **Runtime > Run all** to run every cell from top to bottom.

Colab already includes the required libraries.

## Run on your own computer

1. Open a terminal in `2026-kmitl-data-analytics/`, then create and activate a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate      # Windows: .venv\Scripts\activate
   ```

2. Install the requirements:

   ```bash
   pip install -r requirements.txt
   ```

3. Start the notebook launcher:

   ```bash
   jupyter notebook
   ```

   Then open the notebook you want in the browser page.

## Data

Parts 1–7 need no dataset downloads or manual data files. Their datasets are
created inside the notebooks or built into a library:

- **Part 1:** the **student-score dataset** is created inside the notebook. A CSV
  is written as text in memory and read with `pandas.read_csv`, so no file is
  saved. The **Iris dataset** comes from scikit-learn with `load_iris()` and ships
  with the library.
- **Part 2:** a synthetic **customer dataset** is created in code.
- **Part 3:** a synthetic **house-price dataset** is created in code.
- **Part 4:** **two moons** are created with `make_moons()` and **Iris** is loaded
  with `load_iris()`.
- **Part 5:** balanced and imbalanced classification sets are created with
  `make_classification()`, a small hand example is written in code, and a small
  synthetic regression curve is created in code.
- **Part 6:** `make_blobs()`, `make_moons()`, and small hand-written points show
  compact clusters, curved clusters, and noise.
- **Part 7:** fictional movie ratings and genre features are created in code.

The `data/` folder only holds an explanation. See `data/readme.md`.
