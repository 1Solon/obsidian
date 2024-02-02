## Definition
- **Overfitting** happens when a machine learning model learns the details and noise in the training data to the extent that it negatively impacts the performance of the model on new data.
- This often results in high variance and low bias.

## Causes
1. **Overly Complex Model**: A model with too many parameters relative to the number of observations.
2. **Limited Training Data**: Having a small dataset that does not represent the full scope of the problem domain.
3. **Excessive Training**: Training a model for too long can lead to memorization of the training data.

## Consequences
- **High Training Accuracy but Low Testing Accuracy**: The model performs exceptionally well on training data but poorly on unseen data.
- **Poor Generalization**: The model is unable to perform well on new, unseen data.

## Detection Methods
- **Validation Set Performance**: Monitoring the model's performance on a separate validation dataset.
- **Cross-Validation**: Using cross-validation techniques to assess how the model's predictions generalize to an independent dataset.

## Solutions
1. **Simplify the Model**: Reduce complexity by decreasing the number of parameters or using regularization techniques.
2. **More Training Data**: Increasing the size and diversity of the training dataset.
3. **Early Stopping**: Halting the training process before the model becomes overfitted.

## Example
In a scenario where a decision tree model is used for classification, an overfitted tree might have branches for every possible scenario in the training data, making it overly complex and specific to that particular dataset.

## References
- Bishop, C. M. (2006). Pattern Recognition and Machine Learning. Springer.
- Hawkins, D. M. (2004). The problem of overfitting. Journal of Chemical Information and Computer Sciences.

