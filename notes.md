# AI/ML Bootcamp Notes

---

## 📅 Start Date

**3 Feb 2026**

---

## 🌱 Lecture 1: Introduction to AI, ML & Deep Learning

### Machine Learning

* Machine Learning is about **finding patterns in data**.
* Early ML techniques were limited in capability and scale.

### Deep Learning

* **Deep Learning** is a **subset of Machine Learning**.
* It relies on **neural networks with multiple layers**.

### Key Idea

* Computers **do not understand words**.
* Computers **only understand numbers**.

---

## 📅 4 Feb 2026

## 🧠 Lecture 2: NLP & Transformers

### Word Embeddings

* Words are converted into **vectors (numbers)**.
* Each number represents a **specific dimension of meaning**.
* Similar words have similar vectors.

### RNN Limitations

* RNNs process information **linearly (one word at a time)**.
* They struggle with **long sentences** due to:

  * Sequential processing
  * Limited memory capacity

---

### The Transformer Idea

#### Old Approach

* Process words **one by one**.
* Similar to reading a book from start to finish.

#### New Approach

* Look at **all words in the sentence at the same time**.

#### Attention (Core Idea)

* The model focuses on **most relevant words**.
* Distance between words does **not** matter.

### Transformer Architecture

* Built entirely on the **attention mechanism**.
* Forms the **foundation of Large Language Models (LLMs)**.
* Enables massive **scaling of data and compute**.

### How ChatGPT Works (High Level)

* **Transformer architecture**
* **Large-scale internet data**
* **Next-word prediction**

---

## 🧠 Lecture 3: Neural Networks from Scratch

### Neural Networks

* Neural networks are the **core of deep learning**.
* Training is an **iterative loop**:

  * Guess
  * Measure error
  * Correct
  * Repeat

---

### Neuron (Building Block of AI)

* A neuron is a **tiny decision maker**.
* It is a **simple mathematical function** that:

  * Takes numbers as input
  * Performs basic arithmetic
  * Outputs a signal

#### Components of a Neuron

1. **Inputs**

   * Numerical data (e.g., house size, pixel intensity)

2. **Weights & Summation**

   * Each input has an importance (weight)
   * Inputs are combined into a weighted sum

3. **Bias**

   * Adjusts the neuron’s decision threshold

4. **Activation Function**

   * Decides whether the neuron fires or is suppressed

#### Neuron Formula

```
output = activation( Σ(wᵢxᵢ) + b )
```

---

## 🔘 Activation Functions

### The Linearity Problem

* Without activation functions, networks are **purely linear**.
* Deep networks collapse into a single layer.

### Non-Linear Solution

Activation functions introduce **non-linearity**, which enables:

1. **Breaking Linearity**

   * Adds bends to the math
   * Prevents layers from collapsing

2. **Enabling Depth**

   * Allows learning of complex, multi-layer representations

3. **Universal Approximation**

   * Neural networks can model **any continuous function**

### Common Activation Functions

1. **Sigmoid**

   * S-shaped curve
   * Output range: 0 to 1

2. **Tanh**

   * Output range: -1 to 1

3. **ReLU**

   * Function: max(0, x)
   * Most commonly used

---

## 📉 Loss Function

### Loss

* A **single number** measuring how wrong the model is.
* Lower loss → better predictions
* Training goal → **minimize loss**

### Mean Squared Error (MSE)

```
L = (1/n) Σ(prediction − target)²
```

* Squares make all errors positive
* Large errors are penalized more
* Commonly used for regression tasks

---

## 🔁 Backpropagation

### Concept: Chain of Responsibility

* Error signals flow **backward**:

  * Output layer → Hidden layers → Input layer
* Each weight is adjusted based on:

  * Its contribution to the final error

---

## ⚙️ Learning Rate

* Controls **how fast or slow** the network learns
* Too high → unstable learning
* Too low → very slow learning

---

## 🗺️ Loss Landscape

* Represents error as a surface of hills and valleys
* Training aims to reach the **lowest point (minimum loss)**

---

## ⬇️ Gradient Descent

* Optimization method to **minimize loss**
* Moves weights in the direction of **steepest error reduction**

---

## 🔄 The Training Loop

1. **Forward Pass**

   * Data flows through the network to generate predictions

2. **Calculate Loss**

   * Measure error between prediction and ground truth

3. **Backpropagation**

   * Assign blame to each weight

4. **Update Weights**

   * Use gradient descent to reduce future error

---

## ✅ Final Summary

> A neural network is built by defining layers, passing data forward, calculating loss, and updating weights using gradient descent.
