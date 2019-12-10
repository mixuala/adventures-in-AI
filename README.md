# adventures-in-AI
my personal notes on machine/deep learning


# The Basics
## links
* [glossary](./glossary.md)

## Machine Learning

## Deep Learning

## Reinforcement Learning

## Generative Adversarial Networks



# CNN, Convolutional Neural Networks
## links
* https://adeshpande3.github.io/adeshpande3.github.io/The-9-Deep-Learning-Papers-You-Need-To-Know-About.html

## Basics
CNNs are commonly used on 2D image data.

Images are commonly represented as a series of 2D matrices. An 640x480 pixel RGB image (e.g. BMP, JPG) is represented by one 2D matrix of numbers [0..255] for each color channel, Red/Green/Blue, for a total of 3. The tensor is `shape=(640,480,3)`. A PNG image could optionally have a fourth channel, alpha, which is used to mark transparency, `shape=(640x480,4)`. CNNs typical re-scale the image tensors from [0..255] to [0..1].

Image recognition algorithms must deliver `translation invariance`, e.g. the label/target should be recognized even if it was `translated` (i.e. moved) to another location in the image. For example, a crop that moves the target from the side to the center of the image. CNNs deliver translation invariance through a combination of `convolutions` + `pooling`: 

>a `kernel` (of dimension `NxN`) slides across an image like you are reading a page from a book (left-right and top-bottom), e.g. `convolution`, and only the max or average value of the matrix activation, e.g. `pooling`,  is sent to the next layer.
￼￼![animated convolution](https://miro.medium.com/max/761/1*32zCSTBi3giSApz1oQV-zA.gif)
**Fig. 1:** convolutions of a kernel over a 2D matrix, source: <https://towardsdatascience.com/gentle-dive-into-math-behind-convolutional-neural-networks-79a07dd44cf9>

A `kernel` (a.k.a. `feature` or `channel` in the context of CNN) is a `NxN` matrix of numbers which are learned during training.  A `neuron` is an element in the `NxN` kernel. Each `kernel` is a set of learned weights that slide over specific location in the 2D image tensor, and the dot product of the kernel and matching tensor values are used to calculate activations which are sent to the next layer. 

In the early layers, activations might be for edges or patterns, and in later stages (deeper into the CNN) they might be recognizable concepts like 'fur', 'floppy ears' or 'round thing'. see: <https://distill.pub/2017/feature-visualization/>

## ImageNet, Large-Scale Visual Recognition Challenge
The primary benchmark for image recognition models. Contains a training set of 1000 labeled images of 1000 different classes. Performance is based on Top 5 Error Rate, e.g. the top 5 predictions of correct label for a given image.

**key models**
* AlexNet (2012)
* VGG (2014)
* Inception/GoogLeNet (2015)
* ResNet (2015)



# Reinforcement Learning
## links
* glossary: https://medium.com/@jonathan_hui/rl-reinforcement-learning-terms-242baac11907

# Generative Adversarial Networks, GANS
## links
* (colaboratory) [Style Transfer](https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_2d.ipynb)
* (colaboratory) [Neural Style Transfer](https://colab.research.google.com/github/tensorflow/models/blob/master/research/nst_blogpost/4_Neural_Style_Transfer_with_Eager_Execution.ipynb)
* Draw landscapes [GauGAN AI Art Tool](http://nvidia-research-mingyuliu.com/gaugan)
* Play with GANs [GAN Lab](https://poloclub.github.io/ganlab/)


# Style Transfer
## `gatys` style transfer
**source** <https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/differentiable-parameterizations/style_transfer_2d.ipynb>

![style transfer](https://storage.googleapis.com/tensorflow-lucid/static/img/notebook-styletransfer-diagram.png)
* decodeing style-loss equation, https://miro.medium.com/max/6806/1*kTJm8fSR3n2uooYY0V-vpg.jpeg
* decodeing content-loss equation, https://miro.medium.com/max/2879/1*CVfjP23JUzWKgLIRkf-2Cw.jpeg

## `johnson` with perceptual losses
learn a single pass CNN to replicate the slower optimization step of `gatys` style transfer for a given style target.

![perceptual losses](https://miro.medium.com/max/855/1*TdkNFoecrvBZZbLOHGse0Q.png)

**source** <https://towardsdatascience.com/perceptual-losses-for-real-time-style-transfer-and-super-resolution-637b5d93fa6d>

## parameterization tricks for better style transfer
* non-robust models need parameterization tricks: https://distill.pub/2018/differentiable-parameterizations/
  * for FFT, see also: [Spectral Representations for Convolutional Neural Networks](https://arxiv.org/pdf/1506.03767.pdf)
* `Ulyanov` improvement on fast style transfer, `johnson`
  * instance normalization instead of batch norm, see: https://arxiv.org/pdf/1607.08022.pdf
  * texture networks, see: https://arxiv.org/pdf/1701.02096

## additional works based on Style Transfer
* robust features work better for non-VGG classifiers: [Neural Style Transfer with Adversarially Robust Classifiers](https://reiinakano.com/2019/06/21/robust-neural-style-transfer.html)
* applied to video:
  * [Decrappification, DeOldification, and Super Resolution](https://www.fast.ai/2019/05/03/decrappify/)
  * https://medium.com/@chimezie.iwuanyanwu/real-time-style-transfer-caffa3393833
* Neural Painters, 
  * [Teaching agents to paint inside their own dreams](https://reiinakano.com/2019/01/27/world-painters.html)
  * https://medium.com/libreai/the-joy-of-neural-painting-e4319282d51f
* GAN and HD images, https://towardsdatascience.com/style-transfer-with-gans-on-hd-images-88e8efcf3716







# Stroke-Based Rendering (SBR) ideas
* Neural Painters teach brushstrokes using style-loss, see: https://arxiv.org/pdf/1904.08410.pdf
  notebooks: https://github.com/reiinakano/neural-painters
  * with pyTorch and FastAI, https://medium.com/libreai/the-joy-of-neural-painting-e4319282d51f
  * [Teaching agents to paint inside their own dreams](https://reiinakano.com/2019/01/27/world-painters.html)
* [learning SVG fonts](https://neurohive.io/en/news/new-method-for-generating-svg-fonts-by-google-brain/), see also: https://arxiv.org/pdf/1904.02632.pdf
## raster to vector
* [Potrace](http://potrace.sourceforge.net/)








# Places Challenge
Scene Parsing, Instance Segmentation, Semantic Boundary Detection
* http://placeschallenge.csail.mit.edu/