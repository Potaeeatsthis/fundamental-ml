# Data

This folder does not contain data files. Parts 1–8 need no dataset downloads.
They create data in code or load data built into a library.

Parts 1 to 10 are ready:

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

- **Part 6:** blobs and two moons are created with `make_blobs()` and
  `make_moons()`. Small hand-written points demonstrate distances and density;
  isolated points are added to demonstrate noise.
- **Part 7:** a small fictional movie-rating matrix and genre features are
  created in code. One observed rating per user is held out before fitting.

- **Part 8:** small neuron arrays and all four XOR cases are created in code.
- **Part 9:** Fashion-MNIST is loaded through Keras. The lesson selects 6,000
  training and 1,000 validation images from the original training split, and
  1,000 images from the separate test split.
- **Part 10:** Fashion-MNIST supplies 4,000 training, 800 validation and 800 test
  images using the same split rules. Small filter, pooling and residual examples
  are written in code. Augmentation changes only training views.

Fashion-MNIST needs internet access on the first load (about 30 MB). Keras
normally caches the files in `~/.keras/datasets/`, not in this folder. Neither
lesson requires manual dataset preparation. Part 9 saves model files into a new
temporary directory and prints its location; copy them elsewhere to keep them.

Parts 11 to 14 are planned and have not been created yet.
