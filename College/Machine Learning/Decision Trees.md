## Introduction
---
Decision Trees are a method used in machine learning and data analytics to make predictions or decisions based on data. They involve splitting data into branches to make decisions.

## Key Concepts
---
- **Shannon’s Entropy Model:** Used to measure the uncertainty in the data.
- **Splitting Criteria:** Determines how the data is split at each node.
- **ID3 Algorithm:** A common method for building decision trees.

## Decision Tree Training
---
1. Start with all examples at the root.
2. Perform tests on features to split data into subsets.
3. Repeat the process for each subset until leaf nodes are reached.

## Decision Tree Classification
---
- To classify a new example, it is passed through the tree, following the branches based on its features until it reaches a leaf node.

## Handling Various Feature Types
---
- Decision trees can handle both categorical and continuous features.

## Improving Decision Tree Training
---
- Techniques like pruning are used to avoid overfitting.

## Advantages and Disadvantages
---
- **Advantages:** Interpretable, handles various feature types, robust to noise with pruning.
- **Disadvantages:** Can become large, risk of overfitting, requires retraining for changing concepts.

## Conclusion
---
Decision Trees are a versatile tool in machine learning, useful for both classification and regression tasks, known for their interpretability and ability to handle diverse data types.

## Links
---
* [[Decision Tree - Inductive Bias]]
* [[Information Gain]]
* [[Decision Trees - ID3]]