## Definition
---
- **Euclidean Distance** is a measure of the 'straight line' distance between two points in Euclidean space.
- It's one of the most used distance metrics in machine learning and data analysis.

## Formula
---
- The Euclidean Distance between two points \(P\) and \(Q\) in a Euclidean n-space is defined as:

  \[ d(P, Q) = \sqrt{(q_1 - p_1)^2 + (q_2 - p_2)^2 + \ldots + (q_n - p_n)^2} \]

- Here, \(p_i\) and \(q_i\) are the coordinates of \(P\) and \(Q\) respectively.

## Applications
---
1. **K-Nearest Neighbors (KNN)**: Used to find the nearest neighbors based on Euclidean distance.
2. **Clustering Algorithms**: Like K-Means, where it's used to calculate the distance between data points.
3. **Computer Vision**: For tasks like object detection and facial recognition.

## Characteristics
---
- **Metric Properties**: It satisfies the properties of a metric - non-negativity, identity of indiscernibles, symmetry, and the triangle inequality.
- **Straight-Line Distance**: Represents the shortest path between two points.

## Limitations
---
- **Sensitive to Magnitude**: Can be disproportionately influenced by features that have large magnitudes.
- **Not Scale-Invariant**: Requires normalization of data for effective use in many applications.

## Example
---
In a 2D space, the Euclidean distance between point \(A(2, 4)\) and point \(B(5, 1)\) is calculated as:

  \[ \sqrt{(5 - 2)^2 + (1 - 4)^2} = \sqrt{9 + 9} = \sqrt{18} \]

## References
---
- Deza, E., & Deza, M. M. (2009). Encyclopedia of Distances. Springer.
- Cover, T. M., & Hart, P. E. (1967). Nearest neighbor pattern classification. IEEE Transactions.

