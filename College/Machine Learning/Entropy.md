## Introduction
---
Entropy is a key concept in decision tree algorithms. It represents the level of uncertainty or randomness in a dataset.

## Claude Shannon’s Entropy Model
---
- Entropy measures the purity of a set.
- It quantifies the uncertainty associated with making a random selection from a set.

## Understanding Entropy
---
- Entropy is directly related to the probability of an outcome.
- When the probability of an outcome is high, entropy is low, indicating less uncertainty.
- Conversely, low probability outcomes lead to high entropy, reflecting greater uncertainty.

## Mathematical Representation
---
- Entropy is calculated as the negative logarithm of the probability of an outcome.
- The formula `Entropy = -1 * log(probability)` establishes a relationship where high probability correlates with low entropy and vice versa.

## Significance in Decision Trees
---
- In decision trees, entropy helps in determining the best features for splitting the data.
- Low entropy in a subset implies that the set is pure and vice versa.

## Conclusion
---
Understanding entropy is crucial in decision tree algorithms, as it aids in making more informed decisions about which features to use for data splitting, ultimately affecting the efficiency and accuracy of the model.

## Slides
---
![[Pasted image 20240208114731.png]]
> Node has high Node has low uncertainty uncertainty — High entropy — Low entropy * Entropy is related to the probability of an outcome. * High probability—> Low entropy * Low probability —> High entropy V

![[Pasted image 20240208114747.png]]
> * The log of a probability multiplied by -1 gives the mapping — High probability —> low entropy — Low probability —> high entropy - g’ £° 8., g, : - DUBLIN 0.0 0.2 04 oo 06 08 1.0 0.0 0.2 0.4 oo 06 08 1.0 s )