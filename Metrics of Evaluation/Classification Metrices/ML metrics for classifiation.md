# Confusion Matrix 

A confusion matrix is a performance measurement tool for classification algorithms in machine learning. It's a table that is often used to describe the performance of a classification model (or "classifier") on a set of test data for which the true values are known.

The confusion matrix itself is a square matrix with dimensions equal to the number of classes in the classification problem. For a binary classification problem (with two classes, often denoted as "positive" and "negative"), the matrix is typically 2x2, while for multi-class classification, it can be larger.

```
                 Predicted Class
                |  Positive  |  Negative  |
Actual Class ------------------------------
   Positive     |  True Pos  |  False Neg |
   Negative     |  False Pos |  True Neg  |
```

In a confusion matrix:

- True Positive (TP): These are the cases where the model correctly predicted the positive class.
- True Negative (TN): These are the cases where the model correctly predicted the negative class.
- False Positive (FP): These are the cases where the model incorrectly predicted the positive class when the actual class is negative (also known as Type I error).
- False Negative (FN): These are the cases where the model incorrectly predicted the negative class when the actual class is positive (also known as Type II error).

```
                 Predicted Class
                |    A    |    B    |    C    |
Actual Class ----------------------------------
       A        |   10    |    2    |    3    |
       B        |    1    |   15    |    2    |
       C        |    2    |    1    |   12    |
```

In this confusion matrix:

- For class "A":
  - True Positives (TP) = 10
  - False Negatives (FN) = 2 + 3 = 5 (Misclassified as B or C)
  - False Positives (FP) = 1 + 2 = 3 (Misclassified as B or C)
  - True Negatives (TN) = 15 + 12 = 27 (Correctly classified as B or C)
- For class "B":
  - True Positives (TP) = 15
  - False Negatives (FN) = 1 + 2 = 3 (Misclassified as A or C)
  - False Positives (FP) = 2 (Misclassified as A or C)
  - True Negatives (TN) = 10 + 12 = 22 (Correctly classified as A or C)
- For class "C":
  - True Positives (TP) = 12
  - False Negatives (FN) = 2 + 1 = 3 (Misclassified as A or B)
  - False Positives (FP) = 3 (Misclassified as A or B)
  - True Negatives (TN) = 10 + 15 = 25 (Correctly classified as A or B)

1. **Accuracy**:
   - Accuracy measures the proportion of correctly classified instances among the total instances.
   - Formula: Accuracy = (TP + TN) / (TP + TN + FP + FN)
   - Use: It provides an overall assessment of how often the classifier is correct across all classes. However, it may not be suitable for imbalanced datasets where one class dominates the others.

2. **Precision**:
   - Precision measures the proportion of true positive predictions among all positive predictions made by the model.
   - Out of all instances predicted as postive by the model how many of them are actually positive?
   - Formula: Precision = TP / (TP + FP)
   - Use: Precision is useful when the cost of false positives is high. For example, in medical diagnosis, precision indicates the ratio of correctly identified cases to all cases identified as positive.
   - Precision is about minimizing false positives, ensuring that positive predictions are accurate and relevant.

3. **Recall (Sensitivity)**:
   - Recall measures the proportion of true positive predictions among all actual positive instances in the dataset.
   - Out of all actual positive instances how many of them are correctly predicted by the model as positive.
   - Formula: Recall = TP / (TP + FN)
   - Use: Recall is crucial when missing positive instances is costly. For example, in disease detection, recall indicates the proportion of actual positive cases that were correctly identified.
   - Recall is about minimizing false negatives, ensuring that relevant instances are not missed.
     
4. **F1 Score**:
   - F1 score is the harmonic mean of precision and recall. It balances both precision and recall.
   - Formula: F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
   - Use: F1 score provides a single metric that balances between precision and recall. It's particularly useful when you want to compare models and you need to consider both false positives and false negatives.

5. ROC-AUC
   - For each probability value
     - How many times the model made a good assessment.
     - How many times the model made a wrong assessment.

