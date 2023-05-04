## Cardiotocography Outlier Detection

This project uses the Cardiotocography dataset from the UCI Machine Learning Repository for outlier detection. The dataset contains measurements from fetal heart rate (FHR) and uterine contractions (UC) obtained from cardiotocograms (CTGs) of 2126 fetal observations. 

The goal of this project is to detect outliers in the dataset using principal component analysis (PCA) and clustering-based methods: one-class SVM (oneSVM), isolation forest, local outlier factor (LOF), and density-based spatial clustering of applications with noise (DBSCAN).

### Dataset

The dataset contains 2126 observations with 23 features. Each observation represents a CTG exam and includes the following information:

- FHR baseline (beats per minute)
- Variability of FHR (beats per minute)
- Accelerations per second
- Decelerations per second
- Number of time intervals between contractions
- Average width of the uterine contractions (msec)
- Maximum width of the uterine contractions (msec)
- The strength of the uterine contractions (0-3)
- Histogram features of FHR and UC
- FHR and UC features that quantify the stress level on the fetus.

### Implementation

The project uses PCA to reduce the dimensionality of the dataset and identify the most relevant features for outlier detection. The first two principal components are used to visualize the data and select an appropriate clustering method.

The project uses four clustering-based methods: one-class SVM (oneSVM), isolation forest, local outlier factor (LOF), and density-based spatial clustering of applications with noise (DBSCAN). The methods are used to identify outliers in the dataset and compare their performance.

The project is implemented in Python and uses the following libraries:

- NumPy
- Pandas
- Scikit-learn
- Matplotlib

### Usage

To use this project, clone the repository and run the `outlier_detection.ipynb` notebook. The notebook contains all the code necessary to load the dataset, implement PCA, and apply the clustering-based methods.

Before running the notebook, make sure you have the required libraries installed. You can install them using the following command:

```python
pip install numpy pandas scikit-learn matplotlib
