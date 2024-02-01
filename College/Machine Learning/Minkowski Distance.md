## Definition
---
- **Minkowski Distance** is a generalization of both Euclidean and Manhattan distances. It's a metric in a normed vector space which can be considered as a generalization of both the Euclidean distance and the Manhattan distance.

## Formula
---
- The Minkowski Distance between two points $P$ and $Q$ in an n-dimensional space is defined as:
  $$
  d(P, Q) = \left( \sum_{i=1}^{n} |p_i - q_i|^r \right)^{1/r}
  $$
- Here, $p_i$ and $q_i$ are the coordinates of $P$ and $Q$ respectively, and $r$ is the order of the distance.

## Special Cases
---
- **Euclidean Distance**: When $r = 2$, the Minkowski distance becomes the Euclidean distance.
- **Manhattan Distance**: When $r = 1$, it is the Manhattan distance.

## Applications
---
1. **Machine Learning**: In clustering algorithms and other machine learning algorithms where distance calculation is essential.
2. **Data Mining**: For similarity and dissimilarity measurements between data points.
3. **Computer Graphics**: In digital image processing for various transformations and manipulations.

## Characteristics
---
- **Flexibility**: The parameter $r$ allows flexibility in distance measurement.
- **Metric Properties**: Complies with non-negativity, identity of indiscernibles, symmetry, and the triangle inequality.

## Limitations
---
- **Choosing $r$**: The choice of $r$ can significantly affect the behaviour of the distance metric, and there is no one-size-fits-all choice.
- **Computational Complexity**: Higher values of $r$ can lead to more computational expense.

## Example
---
In a 2D space, for $r = 3$, the Minkowski distance between point $A(2, 4)$ and point $B(5, 1)$ is calculated as:
  $$
  \left( |2 - 5|^3 + |4 - 1|^3 \right)^{1/3} = \left( 27 + 27 \right)^{1/3} = 3 \sqrt[3]{6}
  $$

## References
---
- Deza, E., & Deza, M. M. (2009). Encyclopedia of Distances. Springer.
- Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2009). Introduction to Algorithms. MIT Press.
