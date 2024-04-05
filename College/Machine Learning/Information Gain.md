## Introduction
---
Information Gain (IG) is a crucial concept in decision trees, used for selecting the most informative feature at each step of the tree-building process.

## Definition
---
- Information Gain measures the reduction in [[Entropy]] or uncertainty of a dataset when it is split on a specific feature.
- It quantifies how much more organized or pure the subsets become after the split.

## Calculation
---
- IG is calculated for a descriptive feature \(d\) that splits a dataset of examples into different subsets or partitions.
- The goal is to find the feature that offers the highest information gain, which implies the greatest reduction in entropy.

## Role in Decision Trees
---
- IG is used to decide which feature to test at each node of a tree.
- The feature with the highest IG is chosen as it best splits the dataset into purer subsets.

## Conclusion
---
Information Gain is pivotal in building efficient and accurate decision trees. It helps in choosing the most effective features to split the data, ensuring that the tree captures the most significant patterns in the dataset.

## Slides
---
![[Pasted image 20240208120647.png]]
> * |G for descriptive feature d that splits a dataset D of examples into subsets or partitions {D; , D, , ..., Dy }. IG(d, D) = (original entropy) — (entropy after split) The entropy remaining after the dataset is split using IG(d D) _ H(D) - 7‘em(d D) descriptive feature d 1 H(D) = =Y (P(t;) x log,(P(t;))) T ooy on e saeset i=1 ~ D rem (d, D) = Z = x H (Dy) Each partition is weighted in - |D| —— proportion to its size * N~ entropy of weighting partition D;

![[Pasted image 20240208120725.png]]
![[Pasted image 20240208120739.png]]
![[Pasted image 20240208120749.png]]
![[Pasted image 20240208120757.png]]
![[Pasted image 20240208120810.png]]
