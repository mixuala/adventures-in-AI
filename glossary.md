# Glossary
frequently used terms in machine learning






* activation function
* activation space
* actor-critic
* attention networks
* autoencoder: a pair of 2 connected networks that takes an input, encodes it as a dense set of weights, and then inverts the process with the decoder to reconstruct the original input. Good for replicating images from the sample space. The latent space for encoded vectors may be discontinuous.
* backpropagation 
* Bayes theorem
* bias
* channels
* classification
* cross entropy function
* deep learning 
* depth-wise separable convolution: a tactic to reduce the params of a CNN layer/conv2d by performing a sequence of depth-wise, followed by point-wise (1x1) conv2d, useful for building wider/shallower CNNs for the same number of params. see `tf.layers.separable_conv2d`.  For the same compute cost, downsampling a layer input by a factor of `d` allows for an increase in channels by a factor of `d`.
* dimensionality reduction
* dot-product: “dot product can be viewed as the length of the projected vector a on vector b times the length of the vector b”, proportional to the similarity between vectors
* early stopping
* embedding
* feature engineering
* features
* GANS, generative adversarial networks
* generative
* gradient descent
* gram-matrix: dot product of a matrix. In style-transfer, for a CNN layer with C channels, it is a matrix of shape=(C,C) which represents the similarity between the C channels of the given layer ( the dot product of matrix with shape=(C,WxH) ). The diagonal of the gram matrix has max activation, or (WxH,1)^2. see: https://miro.medium.com/max/1341/1*HeCcGpmxWZFibgLiZCutag.png
* Guassian distribution
* Guassian noice
* hyper plane
* kernel
* latent space
* linear regression:
* linear classifier: a classifier based on a linear combination of feature values. e.g. logistic regression 
* log-likelihood: an function used to simplify the math of gradient descent because, as a monotonically increasing function, log-likelihood changes the slope of the gradient surface, but not the location of the minima.
* logistic regression:
* long-short term memory, LSTM
* loss function
* machine learning
* manifold
* maximum likelihood
* MDP, Markov decision process
* Monte Carlo method
* naive
* normal distribution
* one hot encoding
* optimizer
* over-fitting
* policy gradients
* POMDP, partially observable MDP
* pooling, max pooling
* pre-processing
* precision
* Q-learning
* recall
* receptive field
* regression
* regularization
* reinforcement learning
* ReLU function
* RNN, recurring neural networks
* sigmoid function
* softmax function
* stochastic: same as random
* support vector machine, SVM
* tanh function
* tensor
* test set 
* tractable
* training set
* translation invariance
* under-fitting
* validation set
* variance
* variational autoencoder, VAE: autoencoder where the latent space of encoded vectors is designed to be continuous. This is done by having the encoder output 2 vectors, mu & sigma, and stochastically sampling from the output vectors before decoding.  With a continuous latent space, VAEs can produce generative samples output by sampling and interpolation.

## Robust Features Model
* Robust Model: an `adversarially trained` model, or a model under `standard training` on a constructed `Robust dataset`
* Robust Features: features/channels from a CNN layer (usually last) that activate on patterns that are meaningful to humans and predictive to a label, e.g. fur, eyes, wheels, etc. see `gamma-robustly`. These features are still predictive under adversarial attack. Specifically, they are found by excluding `non-robust features` 
* Non-Robust Features: features/channels from a CNN layer that activate on patterns that are NOT semantically meaningful to humans, but still predictive to a label. However, since they activate on patterns that are not meaninful to humans, their predictions can be easily flipped by adversarial attacks.
* rho-useful Feature: CNN features that are activated/correlated with the prediction of a label for a given dataset. A linear classifier trained on only rho-useful features can deliver non-trivial performance.
* gamma-robustly: a measure of continued `rho-useful(ness)` features when classifying inputs with adversarial perturbations. `gamma-robustly` features are Robust, e.g. still `rho-useful`/predictive of the label under adversarial attack.
* Adversarial attack: a manipulation of an input (image) that is imperceptible to the human eye but still flips a classifier prediction to a different label.

* Robust Training: also `adversarially trained`. training of a classifier to learn `Robust Features` by __preventing__ the learning of `Non-robust features`. This is accomplished by training with a dataset that includes adversarial pertubations and minimizing the `adversarial loss`.

* Adversarial Transferability: predictive capacity of a model when trained on a `Non-robust dataset` that was constructed using a __different__ model

* Robust Dataset: a dataset constructed by optimizing an input to produce the same activations as the `Robust Features` of an adversarially-trained `Robust Model`

