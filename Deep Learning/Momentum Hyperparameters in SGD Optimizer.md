What might happen if you set the momentum hyperparameters close to 1 when using an SGD optimizer?

When setting the momentum hyperparameter close to 1 in Stochastic Gradient Descent (SGD) optimizer, it can lead to some potential effects:

1. Faster convergence: Higher momentum values allow the optimizer to accumulate more past gradients, which can help accelerate convergence. The momentum term acts as a moving average of the gradients, allowing the optimizer to maintain a more consistent direction and speed up the learning process.

2. Smoother optimization trajectory: With higher momentum, the optimizer tends to have a smoother trajectory during optimization. It reduces the oscillations and noise caused by individual gradients, resulting in a more stable and consistent update direction.

3. Overshooting and slower convergence in some cases: While higher momentum can speed up convergence in many cases, setting it too close to 1 can lead to overshooting. If the momentum is too high, the optimizer may overshoot the optimal solution and take longer to converge or even fail to converge. This is especially true if the learning rate is also high, as it can amplify the effect of overshooting.

4. Difficulty in escaping local minima: Higher momentum can make it more challenging for the optimizer to escape local minima. If the momentum is too high, the optimizer may get trapped in a suboptimal solution and struggle to explore other regions of the parameter space.

It's important to note that the optimal value for the momentum hyperparameter depends on the specific problem and dataset. It's generally recommended to start with a lower momentum value (e.g., 0.9) and gradually increase it if necessary, while monitoring the training progress and validation performance. Experimentation and tuning are crucial to finding the right balance between convergence speed and stability.
