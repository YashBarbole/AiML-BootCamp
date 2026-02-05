# AI / ML Bootcamp Notes

Start date: **3 Feb 2026**

---

## Lecture 1 — AI, Machine Learning & Deep Learning

### Machine Learning
- Machine learning is about finding patterns in data.
- Early machine learning methods were limited in capability and scale.

### Deep Learning
- Deep learning is a subset of machine learning.
- It relies on neural networks with multiple layers.

### Core idea
- Computers do not understand words.
- Computers only understand numbers.

---

## Lecture 2 — NLP & Transformers (4 Feb 2026)

### Word embeddings
- Words are converted into vectors (numbers).
- Each number represents a specific dimension of meaning.
- Similar words have similar vector representations.

### Limitations of RNNs
- RNNs process text one word at a time.
- They struggle with long sentences due to:
  - Sequential processing
  - Limited memory capacity

### The transformer idea

Old approach:
- Words are processed one by one.
- Similar to reading a book from start to finish.

New approach:
- All words in a sentence are processed at the same time.

### Attention
- The model focuses on the most relevant words.
- Distance between words does not matter.

### Transformer architecture
- Built entirely on the attention mechanism.
- Forms the foundation of Large Language Models (LLMs).
- Enables massive scaling of data and compute.

### How ChatGPT works (high level)
- Transformer architecture
- Large-scale internet data
- Next-word prediction

---

## Lecture 3 — Neural Networks from Scratch

### Neural networks
- Neural networks are the core of deep learning.
- Training follows an iterative loop:
  - Guess
  - Measure error
  - Correct
  - Repeat

### Neuron (basic unit)
- A neuron is a tiny decision maker.
- It is a simple mathematical function that:
  - Takes numerical inputs
  - Performs basic arithmetic
  - Produces an output signal

### Components of a neuron
- Inputs: numerical data (e.g., house size, pixel intensity)
- Weights: importance assigned to each input
- Bias: shifts the decision threshold
- Activation function: decides whether the neuron fires

Neuron equation:
output = activation( Σ(wᵢxᵢ) + b )

---

## Activation functions

### Why they are needed
- Without activation functions, networks remain linear.
- Deep networks collapse into a single linear transformation.

### Role of non-linearity
Activation functions enable:
- Breaking linearity and preventing layer collapse
- Learning deep, multi-layer representations
- Approximating any continuous function

### Common activation functions
- Sigmoid: output range 0 to 1
- Tanh: output range -1 to 1
- ReLU: max(0, x), most commonly used

---

## Loss and optimization

### Loss
- A single number measuring how wrong the model is.
- Lower loss means better predictions.
- Training objective is to minimize loss.

### Mean Squared Error (MSE)
L = (1/n) Σ(prediction − target)²

- Errors are squared to make them positive.
- Large errors are penalized more.
- Commonly used for regression tasks.

---

## Backpropagation
- Error flows backward from output layer to input layer.
- Each weight is updated based on its contribution to the final error.
- Often described as the chain of responsibility.

---

## Learning rate
- Controls how fast or slow the network learns.
- Too high leads to unstable learning.
- Too low results in slow convergence.

---

## Loss landscape
- Visualizes loss as hills and valleys.
- Training aims to reach the lowest point.

---

## Gradient descent
- Optimization method used to minimize loss.
- Updates weights in the direction of steepest error reduction.

---

## Training loop
1. Forward pass: generate predictions
2. Calculate loss: compare with ground truth
3. Backpropagation: assign error to weights
4. Update weights: reduce future error

---

### Summary
A neural network is built by defining layers, passing data forward, calculating loss, and updating weights using gradient descent.

