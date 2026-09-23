# Data

This folder does not contain data files. Parts 1–5 need no dataset downloads.
They create data in code or load data built into a library.

Parts 1 to 5 are ready:

- **Part 1:** the **student-score dataset** is written as CSV text inside the
  notebook and read with `pandas.read_csv` from a text buffer. No CSV file is
  saved or needed. The **Iris dataset** is loaded with scikit-learn `load_iris()`
  and ships with the library.
- **Part 2:** a synthetic **customer dataset** is created in code, one row per
  customer, with missing values, duplicates, and outliers added on purpose.
- **Part 3:** a synthetic **house-price dataset** is created in code with a fixed
  random seed.
- **Part 4:** **two moons** are created with `make_moons()`, and **Iris** is
  loaded with `load_iris()`.
- **Part 5:** balanced and imbalanced classification sets are created with
  `make_classification()`, a small hand example is written in code, and a small
  synthetic regression curve is created in code.

Parts 6 to 14 are planned and have not been created yet.
