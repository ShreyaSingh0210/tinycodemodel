# TinyCodeLM

A character-level language model trained on Python code, 
built from scratch using PyTorch.

## What is this?
A neural network that learns the patterns of Python code 
character by character and generates new Python code on its own.
Same core idea as GPT and Claude, just at a smaller scale.

## How it works
1. Every character in Python code gets converted to a number
2. The model learns to predict the next character from the previous 32
3. After training, it generates new Python code one character at a time

## Architecture
- Embedding layer: 64 dimensions
- 2 hidden layers: 256 neurons each
- Context window: 32 characters
- Parameters: ~610,000
- Training data: 68,000 characters of Python code

## Results
Loss dropped from 4.12 → 0.0000 over 10,000 training steps.
Model learned to generate syntactically correct Python including
functions, classes, loops, and proper indentation.

## Built with
- Python
- PyTorch
- Google Colab

## Author
Built from scratch as part of my journey toward
building large language models.
