## Definition
---
- **Manhattan Distance**, also known as Taxicab distance or City Block distance, measures the distance between two points in a grid-based path.
- It is the sum of the absolute differences of their Cartesian coordinates.

## Formula
---
- The Manhattan Distance between two points $P$ and $Q$ in an n-dimensional space is defined as:
  $$
  d(P, Q) = \sum_{i=1}^{n} |p_i - q_i|
  $$
- Here, $p_i$ and $q_i$ are the coordinates of $P$ and $Q$ respectively.

## Applications
---
1. **Grid-Based Path Planning**: In urban planning or robotics where paths are grid-like.
2. **Clustering Algorithms**: Like K-Medoids or DBSCAN, which can use Manhattan distance for clustering.
3. **Feature Engineering**: In scenarios where differences in dimensions are more important than the actual distances.

## Characteristics
---
- **Non-Diagonal Movement**: It reflects the sum of horizontal and vertical distances, avoiding diagonal movement.
- **Metric Properties**: Adheres to non-negativity, identity of indiscernibles, symmetry, and the triangle inequality.

## Limitations
---
- **Context-Specific**: More suitable for grid-like path scenarios and might not be ideal for all types of datasets.
- **Different Scale Sensitivity**: Can be sensitive to different scales in various dimensions.

## Example
---
In a 2D grid, the Manhattan distance between point $A(2, 3)$ and point $B(5, 1)$ is calculated as:
  $$
  |2 - 5| + |3 - 1| = 3 + 2 = 5
  $$

## References
---
- Han, J., Kamber, M., & Pei, J. (2011). Data Mining: Concepts and Techniques. Elsevier.
- Preparata, F. P., & Shamos, M. I. (1985). Computational Geometry: An Introduction. Springer.
