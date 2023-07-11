what is batch normalization and why do we use it ?

Batch normalization is a technique used in deep neural networks to normalize the inputs of each layer. It aims to address the internal covariate shift problem, which refers to the change in the distribution of layer inputs during training. By normalizing the inputs, batch normalization helps stabilize and speed up the training process.

Here's why we use batch normalization:

1. Improved Training Speed: Batch normalization helps accelerate the training process by reducing the number of iterations required to converge. It does this by normalizing the inputs to each layer, which reduces the scale of the parameter updates and allows for larger learning rates. This leads to faster convergence and shorter training times.

2. Mitigates the Vanishing/Exploding Gradient Problem: Deep neural networks often suffer from the vanishing or exploding gradient problem, where the gradients become too small or too large during backpropagation. Batch normalization helps alleviate this issue by normalizing the inputs, ensuring that the gradients flow smoothly through the network and preventing them from becoming too small or too large.

3. Reduces Sensitivity to Initialization: Batch normalization makes the network less sensitive to the choice of initial weights. It helps stabilize the learning process by reducing the dependence on the initial parameter values, making it easier to train deep networks.

4. Regularization Effect: Batch normalization acts as a form of regularization by adding a small amount of noise to the network during training. This noise helps prevent overfitting and improves the model's generalization performance.

5. Handles Inputs with Different Scales: Batch normalization normalizes the inputs to each layer, making the network less sensitive to variations in the scale of the input features. This is particularly useful when dealing with datasets where features have different scales, as it helps the network learn more effectively.

Overall, batch normalization is a powerful technique that improves the stability, speed, and generalization performance of deep neural networks. It has become a standard practice in many deep learning architectures and is widely used in various domains, including computer vision, natural language processing, and speech recognition.
