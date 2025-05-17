Attention Is All You Need – Transformer Explained Line by Line
Welcome to this project where we implement the Transformer model from the famous paper Attention Is All You Need — but with a twist.

Instead of just building the model, the goal here is to understand it deeply. Every line of code is written with clarity in mind and explained in detail, making this a learning resource for anyone who wants to really get how Transformers work under the hood.



What This Project Is About
In 2017, the Transformer architecture changed everything in natural language processing. It removed the need for recurrence and convolutions by introducing a mechanism called self-attention, which allows models to process entire sequences in parallel.

This project walks through the core ideas of that paper and shows how to implement them step by step, with detailed explanations for every component.

If you’ve ever tried to read the original paper or understand an existing codebase and felt lost, this repository is for you.



Why did I Build This?

There are plenty of open-source Transformer implementations out there—but most are either:

Too high-level and hide the details behind frameworks, or

Too complex and hard to read for beginners

This project aims to bridge that gap. It focuses on clarity over cleverness. If you're the kind of learner who wants to know how and why things work, you'll feel right at home here.






#Key Components Explained#


Scaled Dot-Product Attention

Calculates attention weights using queries, keys, and values.

Scaling by square root of the dimension to prevent softmax from vanishing gradients.


Multi-Head Attention

Allows the model to jointly attend to information from multiple representation subspaces at different positions.


Positional Encoding

Injects information about the position of tokens in the sequence using sinusoidal functions, as there is no recurrence.


Add & Norm

Residual connections followed by layer normalization to stabilize training.


Feed-Forward Networks

Position-wise fully connected networks applied to each position independently and identically.


Masking

Padding mask and look-ahead mask to prevent attending to future tokens in the decoder during training.
