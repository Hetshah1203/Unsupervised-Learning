# Unsupervised Learning Distance Matrix Analysis

## Overview

This project demonstrates how different **distance metrics** are used in Unsupervised Learning to measure similarity between data points. The notebook applies multiple mathematical distance measures on numerical vectors and medical image data to compare how similarity changes depending on the metric used.

The implementation uses Python libraries such as `scikit-learn`, `NumPy`, and `scikit-image` to compute pairwise distances and analyse image vector similarity.

---

## Objectives

* Understand the role of distance measures in Unsupervised Learning.
* Compute pairwise distances using multiple distance metrics.
* Compare similarity between grayscale medical images by converting them into feature vectors.
* Analyse how different distance metrics influence results.

---

## Distance Metrics Implemented

The notebook explores the following metrics using `sklearn.metrics.DistanceMetric`:

1. **Euclidean Distance**

   * Measures straight line distance between two points.
   * Commonly used in clustering algorithms.

2. **Manhattan Distance**

   * Calculates distance along axes.
   * Useful for grid based data or high dimensional spaces.

3. **Chebyshev Distance**

   * Measures the maximum difference along any coordinate dimension.
   * Often used when movement is allowed in any direction.

4. **Minkowski Distance**

   * Generalized distance metric.
   * Includes Euclidean and Manhattan as special cases.

---

## Methodology

### Step 1: Import Libraries

The project uses:

* scikit-learn for distance metrics
* NumPy for numerical operations
* skimage for image loading and processing

### Step 2: Distance Calculation

Distance metrics are initialized using:

```python
from sklearn.metrics import DistanceMetric
dist = DistanceMetric.get_metric('euclidean')
```

Pairwise distances are computed between vectors.

### Step 3: Image Processing

* MRI images are loaded in grayscale.
* Images are flattened into 1D vectors.
* Distances are calculated between image vectors to measure similarity.

---

## Results and Observations

* Different metrics produce different similarity values for the same data.
* Euclidean distance reflects geometric similarity.
* Manhattan distance performs better when data dimensions increase.
* Chebyshev highlights the largest individual difference between features.
* Image vectors demonstrate how distance metrics can be applied to real world data such as medical imaging.



