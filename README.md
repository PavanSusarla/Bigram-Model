Bigram Language Model (Mini LLM - Stage 1)
📌 Project Overview

This project implements a Bigram Language Model from scratch using Python and PyTorch. It is the first step toward building a Large Language Model (LLM), progressing from simple probabilistic models to advanced architectures like GPT.

The model learns to predict the next character given the current character, i.e.:

P(next_char | current_char)
🚀 Features
Character-level tokenization
Encoding & decoding pipeline
Bigram model using nn.Embedding
Training loop with backpropagation
Text generation using probabilistic sampling
🛠️ Tech Stack
Python 🐍
PyTorch 🔥
NumPy
📂 Project Structure
bigram.ipynb        # Main implementation
wizard_of_oz.txt   # Training dataset
README.md          # Project documentation
⚙️ How It Works
1. Data Preprocessing
Load text data
Extract unique characters (vocabulary)
Map characters to integers
2. Model Architecture
nn.Embedding(vocab_size, vocab_size)
Each character directly maps to logits for next character prediction
3. Training Objective

The model minimizes Cross Entropy Loss between:

Predicted next character
Actual next character
4. Text Generation
Start with an initial token
Predict next character using softmax
Sample from probability distribution
Repeat
📊 Sample Output

Before training:

asdjhaskjdhakjsdh

After training:

The Wizard of Oz was a little girl...

(Note: Output is partially meaningful due to model limitations)

⚠️ Limitations
Only considers one previous character
Cannot capture long-term dependencies
Produces partially coherent text
✅ How to Validate the Model
Loss Decreasing
Loss should reduce over iterations

Output Quality
Should improve gradually with training
📈 Future Improvements
Add context window (n-gram model)
Implement Transformer architecture
Build Mini-GPT
Train on larger datasets
🎯 Learning Outcomes
Understanding probabilistic language models
PyTorch fundamentals
Tokenization & embeddings
Training neural networks from scratch
