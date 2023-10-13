## Positional Encoding
- Process of injecting positional information to the data.
- the sine and cosine functions are used to encode positional information based on the position and feature index. The choice of using sine and cosine functions alternately for even and odd feature
  indices helps to create distinct patterns in the encoding.
- The sine and cosine functions, the positional encoding values for different positions and feature indices will have different frequencies and patterns. This allows the model to capture different
  positional relationships and dependencies within the input sequence.
  
- For Even time step we use the below sine formula to add position information.
<div align="left"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/8ab7ac41f7284da17751933298ca43e2f8d17cc8/image_data%20in%20readme/sine.png"</div>

- For Odd time step we use the below cosine formula to add position information.
<div align="left"><img src="https://github.com/nelson123-lab/my-Data-Science-learnings/blob/bbdfc2f40ae036fbe3d9f076e42c339bc9d8d7b8/image_data%20in%20readme/cosine.png"</div>

- Below is the python implementation for the same.

```python
import torch
import numpy as np

def positional_encoding(x):
    """
    Applies positional encoding to the input tensor.

    Args:
        x (torch.Tensor): Input tensor of shape (batch_size, sequence_length, d).

    Returns:
        torch.Tensor: Tensor with positional encoding of shape (sequence_length, d).
    """
    sequence_length = x.shape[1]
    num_features = x.shape[2]

    # Initialize tensor to store positional encoding values
    positional_encoding = torch.ones(sequence_length, num_features)

    # Calculate positional encoding for each element in the tensor
    for position in range(sequence_length):
        for feature_index in range(num_features):
            # Calculate the positional encoding value based on the position and feature index
            if feature_index % 2 == 0:
                # For even feature indices, use sine function
                positional_encoding[position][feature_index] = np.sin(
                    position / (10000 ** (feature_index / num_features))
                )
            else:
                # For odd feature indices, use cosine function
                positional_encoding[position][feature_index] = np.cos(
                    position / (10000 ** ((feature_index - 1) / num_features))
                )

    return positional_encoding
```
## Common Terminologies
Input sequence dimension of 6 words.
- (6, 512) is dimension of embeddings of each word. (Seq, dmodel)
- dmodel is the size of the embedding vector.
- h = number of heads.
- dk = dv = dmodel/h
- <SOS> - Start of the Sequence
- <EOD> - End of the Sequence
- We are making 3 copies of the inputs as Query, key and value.


- In Multi head attention we alwasys split the Q', K', V' into smaller matrices using the dmodel dimesion so that every head will see the full dimension but a smaller
  part of the embeddings.
