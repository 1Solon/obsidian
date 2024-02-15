## Overview
---
Naive Bayes is a simple yet effective classification algorithm based on Bayes' Theorem with the assumption of independence among predictors. It's particularly known for its effectiveness in text classification.

## Bayes' Theorem
---
Bayes' Theorem provides a way to calculate the probability of a hypothesis given prior knowledge. It is expressed as:

$$ P(A|B) = \frac{P(B|A) \times P(A)}{P(B)} $$

Where:
- $P(A|B)$ is the probability of hypothesis A given the data B.
- $P(B|A)$ is the likelihood of the data under hypothesis A.
- $P(A)$ is the prior probability of hypothesis A.
- $P(B)$ is the normalizing constant.

## Assumptions
---
1. **Feature Independence:** Assumes that all features are independent of each other.
2. **Equal Importance:** Each feature contributes equally to the outcome.

## Types
---
- **Gaussian:** Used when features are continuous and follow a Gaussian distribution.
- **Multinomial:** Good for discrete data and often used in text classification.
- **Bernoulli:** Useful when features are binary.

## Applications
---
- Email Spam Detection
- Sentiment Analysis
- Document Categorization

## Pros
---
- Simple and easy to implement.
- Requires a small amount of training data to estimate parameters.
- Performs well with categorical input variables.

## Cons
---
- Assumes feature independence, which is often not the case.
- Poor estimator.

## Example in Python
---
```python
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score

# Sample dataset
X_train, X_test, y_train, y_test = [Your dataset here]

# Creating and training the model
model = GaussianNB()
model.fit(X_train, y_train)

# Making predictions
predictions = model.predict(X_test)

# Evaluating the model
accuracy = accuracy_score(y_test, predictions)
