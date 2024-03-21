## Introduction to Evaluation
Evaluation plays a crucial role in machine learning by estimating model performance upon deployment and comparing different models. The process involves selecting appropriate measures, running models on datasets, and comparing results to benchmarks, tailored to the hypothesis being tested.

---

## Hypothesis Testing
Formally examines two opposing hypotheses, null (𝐻₀) and alternative (𝐻₁), where 𝐻₀ assumes no difference between two models' performance. Hypotheses testing is critical for validating model improvements or comparing different models' effectiveness.

---

## Error Types
- **Type I Error (False Positive)**: Incorrectly rejecting the true null hypothesis.
- **Type II Error (False Negative)**: Failing to reject a false null hypothesis.
Costs associated with these errors vary based on the hypothesis context, impacting decisions significantly.

---

## Standard Evaluation Approach
Utilizes a labelled test set to compare actual outcomes against model predictions. It's essential to use separate datasets for training and testing to ensure realistic accuracy and model generalization.

---

## Performance Measures
While no model is perfect, alignment of evaluation measures with the task at hand is crucial. Measures range from simple accuracy to more complex ones like Precision, Recall, and F1-Score, depending on the model’s application area and requirements.

---

## Confusion Matrix and Related Measures
A confusion matrix offers a detailed breakdown of prediction performance, leading to measures like True Positive Rate (Sensitivity) and True Negative Rate (Specificity), among others. These measures help in understanding model performance beyond mere accuracy.

---

## Precision and Recall
Originating from information retrieval, these measures assess the relevance of model predictions. Precision measures the proportion of correct positive identifications, while Recall measures the proportion of actual positives correctly identified.

---

## Dealing with Imbalanced Data
Imbalanced datasets, where some classes are underrepresented, can mislead performance evaluation. Balanced Accuracy Rate (BAR) and Balanced Error Rate (BER) offer more nuanced insights into model performance across diverse class distributions.

---

## Evaluation Methodologies
- **Hold-Out Method**: Splits the dataset into training, validation, and test sets.
- **Cross-Validation**: Enhances reliability by using multiple splits and aggregating performance across folds.
- **Bootstrapping**: Useful for very small datasets, involving random sampling with replacement to assess performance.

---

## Selecting Performance Measures
Choice of performance measure is informed by the problem nature, data characteristics, and domain-specific needs. Recommendations include Average Class Accuracy for classification tasks and R² Coefficient for regression.

---

## Summary
Evaluation in machine learning encompasses selecting suitable performance measures, understanding error types, and applying appropriate methodologies to assess model effectiveness. The aim is to ensure models perform well in practical applications, not just under test conditions.

---
* [[ML Lecture 5]]
