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

