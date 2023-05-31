WHat is Overfitting ?
- Overfitting is a common problem in machine learning where a model is trained too well on the training data, to the point that it starts to memorize the data         instead of learning the underlying patterns. This results in a model that performs well on the training data but poorly on new, unseen data.

What is Regulariztion and what are the different types ?
- Regularization is a technique used to prevent overfitting by adding a penalty term to the loss function of the model. This penalty term discourages the model from   fitting the training data too closely and encourages it to learn the underlying patterns instead. There are several regularization techniques, but two of the most   popular ones are L1 regularization and L2 regularization.
- L1 regularization, also known as Lasso regularization, adds a penalty term to the loss function that is proportional to the absolute value of the model weights.     This results in a sparse model where some of the weights are set to zero, effectively removing some of the features from the model.
- L2 regularization, also known as Ridge regularization, adds a penalty term to the loss function that is proportional to the square of the model weights. This         results in a model where all the features are used, but the weights are smaller and more evenly distributed.

What is bias-Vairance Tradeoff ?
- The bias-variance tradeoff is a fundamental concept in machine learning that refers to the tradeoff between the ability of a model to fit the training data well     (low bias) and ability to generalize to new, unseen data (low variance).
- Bias refers to the error that is introduced by approximating a real-world problem with a simplified model. A model with high bias is too simple and may not capture   the underlying patterns in the data, resulting in underfitting.
- Variance, on the other hand, refers to the error that is introduced by the model's sensitivity to small fluctuations in the training data. A model with high         variance is too complex and may fit the training data too closely, resulting in overfitting.
- The goal of machine learning is to find a model that has low bias and low variance, which means that it can fit the training data well and generalize to new data.   However, there is always a tradeoff between bias and variance.
- If we increase the complexity of the model, we can reduce bias and improve its ability to fit the training data well. However, this also increases the model's       sensitivity to small fluctuations in the data, which increases variance and reduces its ability to generalize to new data.
- On the other hand, if we decrease the complexity of the model, we can reduce variance and improve its ability to generalize to new data. However, this also           increases bias and reduces its ability to fit the training data well.
- Therefore, the key to finding the right balance between bias and variance is to choose a model that is complex enough to capture the underlying patterns in the       data but not so complex that it overfits the training data. This can be achieved through techniques such as cross-validation, regularization, and ensemble methods.

How do you handle data imbalance issues?
- Data imbalance is a common problem in machine learning where the number of instances in one class is much higher than the number of instances in another class.   This can lead to biased models that perform poorly on the minority class. There are several techniques that can be used to handle data imbalance issues:

  1. Resampling: This involves either oversampling the minority class or undersampling the majority class to balance the number of instances in each class.            Oversampling can be done by duplicating instances from the minority class, while undersampling can be done by randomly removing instances from the majority        class.

  2. Synthetic data generation: This involves generating synthetic data for the minority class using techniques such as SMOTE (Synthetic Minority Over-sampling        Technique) or ADASYN (Adaptive Synthetic Sampling). These techniques create new instances for the minority class by interpolating between existing instances.

  3. Cost-sensitive learning: This involves assigning different misclassification costs to different classes. This can be done by adjusting the class weights in        the loss function of the model.

  4. Ensemble methods: This involves combining multiple models to improve the performance on the minority class. This can be done by training multiple models on        different subsets of the data or by using techniques such as bagging or boosting.

  5. Anomaly detection: This involves treating the minority class as an anomaly and using anomaly detection techniques to identify instances that belong to the        minority class.

  The choice of technique depends on the specific problem and the characteristics of the data. It is important to evaluate the performance of the model on both     the majority and minority classes to ensure that the model is not biased towards one class.


