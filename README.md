# Variational-Autoencoders

### Project for the course Machine Learning for Graphs and Sequential Data(IN2323) at Technical University of Munich. 

A variational autoencoder consists of an encoder, a decoder, and a loss function. 
The encoder is a neural network which produces the parameters of variational distribution. The input to the encoder is a datapoint <img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{\x}^{(i)} \in \mathbb{R}^D"> and its output is a hidden representation <img src="https://render.githubusercontent.com/render/math?math=\mathbf{z}^{(i)}">. 
The decoder is another neural network that takes <img src="https://render.githubusercontent.com/render/math?math=\mathbf{z}^{(i)}"> and produces the parameters <img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{\theta}^{(i)} \in \mathbb{R}^D"> of the data likelihood <img src="https://render.githubusercontent.com/render/math?math=p_{\boldsymbol{\theta}^{(i)}}(\mathbf{x}^{(i)}|\mathbf{z}^{(i)})">
Finally, the ELBO function is computed as follows:

<img src="https://render.githubusercontent.com/render/math?math=\mathcal{L}_i(\boldsymbol{\psi}, \boldsymbol{\lambda}) = \mathbb{E}_{\mathbf{z}^{(i)} \sim q_{\boldsymbol{\phi}^{(i)}} (\mathbf{z}^{(i)})}\left[\log p_{\boldsymbol{\theta}^{(i)}}(\mathbf{x}^{(i)} | \mathbf{z}^{(i)})\right] - \mathbb{KL}(q_{\boldsymbol{\phi}^{(i)}}(\mathbf{z}^{(i)}) || p(\mathbf{z}))">
