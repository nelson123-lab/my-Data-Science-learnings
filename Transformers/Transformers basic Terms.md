Positional Encoding


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
