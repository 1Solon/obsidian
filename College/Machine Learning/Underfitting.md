## Definition
- **Underfitting** occurs when a machine learning model is too simplistic to capture the underlying patterns in the data.
- It often results in poor performance on both training and testing datasets.

## Causes
1. **Overly Simple Model**: The model lacks the necessary parameters or structure to learn from the data.
2. **Insufficient Training**: Not enough training time or data to allow the model to learn the complexities.
3. **Poor Feature Selection**: Inadequate or irrelevant input features can hinder the model's learning capability.

## Consequences
- **Low Training Accuracy**: The model performs poorly even on the training data.
- **Poor Generalization**: Inability to predict or classify new data effectively.

## Detection Methods
- **Training vs Validation Performance**: Comparing performance metrics on both training and validation datasets.
- **Learning Curves**: Analysing the learning curves for signs of underfitting, like persistently high error rates.

## Solutions
1. **Increase Model Complexity**: Adding more parameters or using a more sophisticated model.
2. **Feature Engineering**: Improving the input features through techniques like feature selection or transformation.
3. **Additional Training Data**: Providing more varied or comprehensive data for training.

## Example
Consider a dataset with nonlinear patterns. Using a linear regression model on this data can lead to underfitting, as the linear model is too simplistic to capture the non-linear relationships.

## References
- James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). An Introduction to Statistical Learning. Springer.
- Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. MIT Press.

