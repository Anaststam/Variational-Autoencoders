# Variational-Autoencoders

### Project for the course Machine Learning for Graphs and Sequential Data(IN2323) at Technical University of Munich. 

A variational autoencoder consists of an encoder, a decoder, and a loss function. 
The encoder is a neural network which produces the parameters of variational distribution. The input to the encoder is a datapoint x and its output is a hidden representation z. 
The decoder is another neural network that takes samples z and produces the parameters θ of the data likelihood. 
Finally, ELBO function is computed as follows:

$$\mathcal{L}_i(\boldsymbol{\psi}, \boldsymbol{\lambda}) = \mathbb{E}_{\mathbf{z}^{(i)} \sim q_{\boldsymbol{\phi}^{(i)}} (\mathbf{z}^{(i)})}\left[\log p_{\boldsymbol{\theta}^{(i)}}(\mathbf{x}^{(i)} | \mathbf{z}^{(i)})\right] - \mathbb{KL}(q_{\boldsymbol{\phi}^{(i)}}(\mathbf{z}^{(i)}) || p(\mathbf{z}))$$
