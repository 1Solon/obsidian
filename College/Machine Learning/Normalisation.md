## Definition
---
- **Normalization** is a process in data preparation to adjust the range of data values so that they can be compared on a common scale.
- It is often used to improve the performance and accuracy of machine learning algorithms.

## Purpose
---
1. **Scale Features to a Uniform Range**: This includes scaling the features to a range like 0 to 1 or -1 to 1.
2. **Improve Convergence in Training**: Helps in faster convergence during the training of models.
3. **Reduce Impact of Outliers**: Minimizes the influence of outlier values in the data.

## Common Methods
---
1. **Min-Max Normalization**: Transforms features by scaling each feature to a given range, typically [0, 1].
2. **Z-Score Normalization (Standardization)**: Adjusts the features so they have the properties of a standard normal distribution with μ = 0 and σ = 1.
3. **Decimal Scaling**: Moves the decimal point of values of the feature.

## Application
---
- Widely used in data pre-processing for machine learning and deep learning models.
- Particularly important in algorithms that use distance measures like K-Nearest Neighbours (KNN) and Gradient Descent based techniques.

## Example
---
Consider a dataset with two features: age (ranging from 1 to 100) and income (ranging from 20,000 to 100,000). Normalization adjusts these features into a similar scale, enabling a more balanced and fair comparison in models.

## References
---
- Han, J., Pei, J., & Kamber, M. (2011). Data Mining: Concepts and Techniques. Elsevier.
- Jolliffe, I. T., & Cadima, J. (2016). Principal component analysis: a review and recent developments. Philosophical Transactions of the Royal Society A.

