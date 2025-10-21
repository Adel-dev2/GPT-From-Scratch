# GPT-From-Scratch

This repository contains a PyTorch implementation of a GPT-like language model built from scratch. The model uses transformer blocks with multi-head self-attention, feed-forward layers, dropout, and layer normalization. It's trained on the Tiny Shakespeare dataset to generate Shakespearean-style text. The notebook handles data fetching, encoding, batching with DataLoader, training, and text generation.

## Overview
- **GPT_FromScratch.ipynb**: Fetches Tiny Shakespeare data, builds vocabulary (character-level), creates a custom Dataset/DataLoader, defines model components (Head, MultiHeadAttention, FeedForward, TransformerBlock, GPTLanguageModel), trains for 10 epochs, and generates text.
- Hyperparameters: 4 layers, 192 embeddings, 3 heads, batch size 32, block size 128, learning rate 1e-3, dropout 0.1.
- Device: GPU (CUDA) if available, else CPU.
