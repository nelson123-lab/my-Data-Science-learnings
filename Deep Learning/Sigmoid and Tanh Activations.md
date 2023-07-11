Why sigmoid and tanh is not preferred to be used as the activation function is the hidden layer of the neural network?

Sigmoid and tanh activation functions were commonly used in the past for hidden layers in neural networks. However, they have certain limitations that make them less preferred compared to other activation functions, such as ReLU (Rectified Linear Unit), in modern neural network architectures. Here are a few reasons why sigmoid and tanh activation functions are not commonly used in hidden layers:

1. Saturation and Vanishing Gradients: Sigmoid and tanh activation functions saturate at the extreme ends of their input range, causing the gradients to become very small. This can lead to the vanishing gradient problem, where the gradients diminish as they propagate backward through the network layers. As a result, the network may struggle to learn effectively, especially in deep networks with many layers.

2. Limited Output Range: Sigmoid activation function outputs values between 0 and 1, while tanh activation function outputs values between -1 and 1. This limited output range can cause the activations to be concentrated around the extremes, making it harder for subsequent layers to learn and update their weights effectively. It can also lead to slower convergence and suboptimal learning.

3. Non-Centered Output: Both sigmoid and tanh activation functions are not centered around zero. This can introduce bias in the network, as the activations are shifted towards the positive or negative end of the range. This bias can hinder the learning process and make it more challenging for the network to converge.

4. Computational Efficiency: Sigmoid and tanh activation functions involve expensive exponential calculations, which can be computationally inefficient, especially when dealing with large-scale neural networks and big datasets. Activation functions like ReLU, on the other hand, involve simpler operations, making them computationally more efficient.

In contrast, activation functions like ReLU have gained popularity in hidden layers due to their advantages. ReLU does not suffer from saturation, avoids the vanishing gradient problem, has a larger output range, and is computationally efficient. These properties make ReLU and its variants (e.g., Leaky ReLU, Parametric ReLU) more suitable for deep neural networks, enabling faster training and better performance.

It's important to note that the choice of activation function depends on the specific task, dataset, and network architecture. While sigmoid and tanh activation functions may still have applications in certain scenarios, their limitations in deep networks have led to the preference for other activation functions like ReLU.
