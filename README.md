Bigram Language Model
📌 Overview

This project implements a basic Bigram Language Model using Python and PyTorch.
The model learns to predict the next character based on the current character.

🚀 Features
Character-level text processing
Simple neural network using PyTorch
Training with cross-entropy loss
Text generation from trained model

🛠️ Tech Stack
Python
PyTorch

⚙️ How It Works
Convert text into characters
Map characters to numbers
Train model to predict next character
Generate text using learned probabilities

▶️ Run the Project

Install dependencies:

pip install torch

Run the notebook:

bigram.ipynb
📊 Output
Initially generates random text
Improves slightly after training
Still limited due to simple bigram approach
⚠️ Limitation
Only looks at one character at a time
Cannot understand full sentences
🎯 Learning
Basics of language models
PyTorch training workflow
Text generation concepts
