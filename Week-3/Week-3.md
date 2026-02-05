# AI / ML Bootcamp Notes

## Week 3 — Tokenization, Embeddings & Transformers  
**Date: 5 Feb 2026**

---

## Character-level vs Word-level Approaches

### Character-level approach
- Text is split into individual characters.
- Very small vocabulary.
- Sequences become very long and inefficient.

### Word-level approach
- Text is split into full words.
- Shorter sequences.
- Cannot handle unseen or rare words well.

---

## Tokenization in Transformer Models

### Tokenization
- Converts text into tokens.
- Tokens are mapped to numerical IDs.
- Models understand only numbers, not raw text.

---

## Byte Pair Encoding (BPE)

### What it is
- Algorithmic method to construct tokens.
- Starts with characters and merges frequent pairs.

### Why BPE is used
- Handles unknown words.
- Keeps vocabulary size reasonable.
- Used in modern NLP systems.

---

## Tokenization in Modern Practice
- Uses subword-level tokens.
- Common words → single token.
- Rare words → split into smaller pieces.

---

## Why Tokenization Matters
- Affects model understanding.
- Impacts efficiency and memory usage.
- Influences training and inference speed.

---

## Thinking Models (High Level)
- Models designed to reason step-by-step.
- Focus on correctness rather than fast guessing.
- Examples include advanced reasoning LLMs.

---

## Embeddings

### What embeddings are
- Tokens are converted into vectors.
- Each vector captures semantic meaning.
- Similar meanings result in similar vectors.

### Embedding matrix
- Large table of learned vectors.
- One vector per token.
- Learned during training.

---

## Practical Understanding of Embeddings
- Simulated an embedding matrix.
- Observed real learned embeddings.
- Understood token-to-vector mapping.

---

## Positional Encoding

### Why it is needed
- Transformers process all tokens in parallel.
- Word order would be lost without position info.

### What it does
- Adds positional information to embeddings.
- Helps model understand sequence order.

---

## Transformer Input Pipeline

1. Tokenization → text to token IDs  
2. Embedding → token IDs to vectors  
3. Positional embedding → add order information  

---

### Summary
Transformer models rely on tokenization, embeddings, and positional encoding to convert text into meaningful numerical representations for attention-based learning.
