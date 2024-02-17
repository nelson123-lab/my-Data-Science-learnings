## Bias and Variance:

- **Bias**:
  - Definition: The simplifying assumptions made by the model to make the target function easier to approximate.
  - Low Bias: When the model can capture true relationships between the data points.
  
- **Variance**:
  - Definition: The difference in fits between data sets is called variance.
  - The amount that the estimate of the target function will change given different training data.

### Underfitting:
- **Characteristics**:
  - High bias and low variance.
  - Predictions are average in all cases but never great.
  - Refers to a model that can neither model the training data nor generalize to new data.

### Overfitting:
- **Characteristics**:
  - Low bias and high variance.
  - Fits the training set really well but not the testing set.

### Finding the Sweet Spot:
- **Methods**:
  1. **Regularization**: Introducing a penalty on the complexity of the model to avoid overfitting.
  2. **Boosting**: Building multiple weak learners sequentially to create a strong learner, reducing bias and variance.
  3. **Bagging**: Creating multiple models using subsets of the training data and aggregating their predictions to reduce variance.

### Trade-off:
- **Definition**: Tension between the error introduced by the bias and the variance.

## Bias and Variance of different machine learning models

| Algorithm               | Bias       | Variance   | Description                                                                                   |
|-------------------------|------------|------------|-----------------------------------------------------------------------------------------------|
| Linear Regression       | High       | Low        | Assumes linear relationship, may underfit complex data.                                        |
| Decision Trees          | Low        | High       | Can represent complex boundaries, prone to overfitting noisy data.                             |
| K-Nearest Neighbors     | Low        | High       | Makes few assumptions, can overfit with small values of K.                                      |
| Support Vector Machines | Low        | High       | Can capture intricate relationships, may overfit without proper tuning or with small datasets. |
| Logistic Regression     | Moderate   | Moderate   | Assumes linear relationship, moderate capacity to capture nonlinearity.                         |
| Random Forests          | Moderate   | Moderate   | Ensemble method reduces variance compared to individual trees.                                 |
| Gradient Boosting Machines | Moderate | Moderate | Sequentially fits trees to residuals, balances bias and variance through boosting.              |
| Neural Networks         | Variable   | Variable   | Highly flexible, bias-variance trade-off depends on architecture, regularization, and data.    |

