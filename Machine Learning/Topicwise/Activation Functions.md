## Activation function

Activation functions are a crucial component of neural networks. They introduce non-linearities into the network, enabling it to learn complex patterns and relationships in data. Here are some key uses of activation functions:

1. Introducing Non-Linearity: Activation functions introduce non-linear transformations to the output of a neuron. Without activation functions, the neural network would effectively reduce to a linear model, unable to learn complex patterns.

2. Facilitating Gradient Descent: Activation functions enable backpropagation, the algorithm used to train neural networks by adjusting the weights based on the error between predicted and actual outputs. They allow gradients to flow backward through the network, facilitating the optimization process.

3. Enabling Neural Networks to Approximate Any Function: A neural network with non-linear activation functions can approximate any continuous function to arbitrary accuracy, given enough hidden units (neurons) and layers. This property is known as the Universal Approximation Theorem.

4. Handling Complex Relationships: Non-linear activation functions allow neural networks to learn and represent complex relationships in data, such as patterns in images, sequences in text, or trends in numerical data.

Common activation functions include:
- **Sigmoid**: S-shaped curve, squashes input values between 0 and 1.
- **Hyperbolic Tangent (tanh)**: Similar to sigmoid but squashes input values between -1 and 1.
- **Rectified Linear Unit (ReLU)**: Linear for positive inputs, zero for negative inputs.
- **Leaky ReLU**: Similar to ReLU but allows a small, non-zero gradient for negative inputs to mitigate the dying ReLU problem.
- **Exponential Linear Unit (ELU)**: Similar to ReLU but with smoother outputs for negative inputs.
- **Softmax**: Used in the output layer of classification neural networks to produce probabilities for each class.
