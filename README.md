# MNIST Digit Classifier — From Scratch

A neural network built from scratch using only NumPy. No PyTorch, no TensorFlow, no ML frameworks just math and matrix operations.

## Architecture
- Input layer: 784 neurons (28×28 pixels flattened)
- Hidden layer: 128 neurons + ReLU activation
- Output layer: 10 neurons + Softmax activation

## Results
| | Accuracy |
|---|---|
| Training | 90.27% |
| Test | 90.78% |

Trained for 500 epochs using gradient descent.

## What's implemented from scratch
- Forward propagation
- Backpropagation using chain rule
- Gradient descent weight updates
- ReLU and Softmax activations
- Cross entropy loss
- One-hot encoding
- Custom handwritten digit prediction

## Run it
```bash
pip install numpy matplotlib pillow
```
Open `mnist.ipynb` in VS Code or Jupyter and run all cells.

## Test your own handwriting
Write a digit on paper, photograph it, crop to just the digit and save as a png in the project folder. Then run:
```python
predict_custom('your_image.png')
```

## Why from scratch?
To understand what frameworks like PyTorch are actually doing under the hood. Every line maps directly to the math — no black boxes.

## Dataset
Download MNIST from: https://ossci-datasets.s3.amazonaws.com/mnist/
Place the 4 ubyte files in the project root.
