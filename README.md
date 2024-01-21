# TransformerNeuralNetwork
this is the architecture by which modern LLMs like chatGPT are built on

# Transformer Neural Network

This project implements a Transformer neural network architecture for sequence-to-sequence modeling. It contains implementations of the Encoder, Decoder, and full Transformer model.

## Files

- `transformer.py` - Main source code with Transformer model implementation 
- `README.md` - This read me file

## Model Architecture

The Transformer model utilizes Encoder and Decoder blocks that rely primarily on attention mechanisms rather than recurrence.

Some key components:

- Multi-headed self attention layers 
- Layer normalization  
- Position wise feed forward networks
- Residual connections around each block

The model takes in a source sequence and generates an output target sequence.

## Usage

The script provides a simple example of initializing a Transformer model and passing sample input for demonstration.

To use the model:

```python
src = sample_input_ids 
trg = sample_target_ids

model = Transformer(params)
output = model(src, trg[:,:-1])
```

See the __main__ section for details.

The source and target sequences, padding indices, vocab sizes etc. need to be set appropriately. The model is setup for sequence-to-sequence tasks.

## References

Refer the original [Attention Is All You Need](https://arxiv.org/abs/1706.03762) paper for details on the Transformer architecture.

## Contributing

Pull requests are welcome for improvements and enhancements!
