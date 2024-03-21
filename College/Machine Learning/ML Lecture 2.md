## Overview
This lecture dives into similarity-based learning, focusing on the k-Nearest Neighbors (kNN) algorithm. It covers the fundamental concepts of feature space, similarity measures, and various types of data, moving on to detailed discussions on distance metrics, normalization, and prediction techniques.

---

## Big Idea
Similarity-based learning, exemplified by kNN, relies on historical instances to make predictions for new queries. This method is inspired by the human ability to learn from past experiences.

---

## Fundamentals of Similarity Learning

### Feature Space
- Defined as a D-dimensional space where each axis represents a feature of the data.
- Allows visualization of the relationship between instances based on their features.

### Similarity Measures
- The core of kNN is determining how "close" or similar two instances are, typically using distance metrics like Euclidean or Manhattan distance.

---

## Distance Metrics
- **Euclidean Distance**: The most common measure, calculating the straight-line distance between two points.
- **Manhattan Distance**: Computes the sum of absolute differences between points in all dimensions, resembling a "city block" distance.
- **Minkowski Distance**: A generalization of Euclidean and Manhattan distances, adjustable with a parameter `p`.

---

## Handling Different Types of Data
- **Binary**: Features with two possible values (e.g., True/False).
- **Categorical (Nominal)**: Features with a set of discrete values with no intrinsic order.
- **Ordinal**: Similar to categorical, but with an inherent order among the values.
- **Interval**: Numeric values that allow for ordering and subtraction.

---

## Nearest Neighbour Algorithm (k-NN)
1. **Basic Concept**: Classify a query instance based on the most similar historical instances.
2. **Distance Calculation**: Compute the distance from the query to each instance in the training set.
3. **k Selection**: Choose the `k` nearest instances and use their majority class for prediction.
4. **Weighted k-NN**: Assign more weight to nearer neighbours, potentially improving accuracy.

---

## Data Normalization
- Crucial for ensuring that no single feature dominates the distance calculation due to its scale.
- Techniques like min-max normalization adjust features to a common scale.

---

## Predicting Continuous Targets
- k-NN can also predict continuous values by averaging the targets of the `k` nearest neighbours.

---

## Algorithm Characteristics
- k-NN is a "lazy learning" technique, constructing the model at classification rather than training time.
- Requires careful selection of `k` to balance sensitivity to noise against the risk of oversimplifying the model.
- Data normalization is essential for effective distance calculation.

---

## Tools and Resources
- **Kaggle**: A platform for data science competitions and datasets.
- **Scikit-learn's Nearest Neighbor module**: Provides efficient tools for conducting k-NN analyses.

[Scikit-learn Nearest Neighbor](https://scikit-learn.org/stable/modules/neighbors.html)

---

## Other notes:
* [[ML Lecture 1]]
* "Learn something valuable from the dataset"
* "Volume of data is low, we end up with [[Underfitting]]"
* "Volume of data is high, need to be careful about [[Overfitting]]"
* [[Similarity Learning]]
* Important concept: [[Normalisation]]