## How Tensorflow works

1. **TensorFlow and Computational Graphs**: 
   - TensorFlow operates on the principle of computational graphs. These graphs represent mathematical computations as a series of interconnected nodes. Each node represents an operation, and the edges between nodes represent the flow of data, typically in the form of tensors (multi-dimensional arrays). 

2. **Dynamic Graph Creation with Inputs**: 
   - Computational graphs in TensorFlow are dynamically constructed when inputs are passed through the network. This means that the structure of the graph can vary depending on the input data and the operations applied to it. This flexibility allows TensorFlow to handle various types of data and model architectures efficiently.

3. **Tensor Flow Through Graphs**:
   - The inputs to TensorFlow models are typically multidimensional tensors. These tensors flow through the computational graph, undergoing various mathematical operations at each node. As they traverse the graph, they undergo transformations until they reach the output nodes, where the final results are produced. This flow of tensors through the graph is where TensorFlow gets its name.
