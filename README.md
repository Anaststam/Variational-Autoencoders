# Variational-Autoencoders

### Project for the course Machine Learning for Graphs and Sequential Data(IN2323) at Technical University of Munich. 

A variational autoencoder consists of an encoder, a decoder, and a loss function. 
The encoder is a neural network which produces the parameters of variational distribution. The input to the encoder is a datapoint x and its output is a hidden representation z. 
The decoder is another neural network that takes samples $\mathbf{z}}$ and produces the parameters $\boldsymbol{\theta}^{(i)} \in \mathbb{R}^D$ of the data likelihood $p_{\boldsymbol{\theta}^{(i)}}(\mathbf{x}^{(i)}|\mathbf{z}^{(i)})$.
