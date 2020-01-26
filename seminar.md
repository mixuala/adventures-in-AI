## TOC
1. [Basics](#basics)
2. [Colab notebooks](#colab-notebooks)
3. [Quotes](#quotes)
4. [Interesting](#interesting)
5. [Headlines](#headlines)
6. [Ethics and Issues](#ethics-and-issues)
7. [Glossary](#glossary)


## Big Picture ##

1. What's the big deal?
  ![word cloud](https://iiot-world.com/wp-content/uploads/2017/05/word-cloud.png)
  - Through A.I. and Machine Learning, computers are making decisions that affect your lives, both everyday and into the future. 
  - How are you touched by AI?
    - IG feeds, advertising, suggestions
    - siri, alexa, hey google voice assistants
    - snapchat filters, face detection,
    - grammarly,
  - Others  
    - Cambridge Analyica uses AI and Facebook Ads to tip the 2016 elections and elect Donald Trump as POTUS
    - Self-driving cars
  
1. What is AI and Machine Learning?
  - Computer Science: program algorithms to do things step-by-step
  - Machine Learning is the practice of teach computers to make decisions by showing it data



  

1. machine learning is making decisions that affect your lives
  AI beats humans at: chess, go, StarcraftII, Dota2, rubiks cube

1. deep learning basics
  1. data, data, data
  2. deep, deeper, deepest, the power of n-dimensions
		* [Matthieu Robert-Ortis](https://cargocollective.com/matthieu-robert-ortis)
|___|___|		
|[!["Epigénétique"](https://i.postimg.cc/R04G6B70/IMG-3317.jpg =240x360)](https://www.youtube.com/watch?time_continue=8&v=vwF7AHTQaoc)|[![animals](https://i.postimg.cc/8zhtz5r3/IMG-3319.jpg =240x360)](https://youtu.be/7SnLKq5b5Y0?time_continue=8)|

1. deep learning progress: better, smaller, faster
  see: https://interestingengineering.com/11-times-ai-beat-humans-at-games-art-law-and-everything-in-between
  - VGG > Inception > Resnet
  - RNN > LSTM > attention networks
  - RL: DeepMind: AlphaGo, AlphaStar, AlphaZero, StarcraftII/Dota2
    see: https://deepmind.com/blog/article/alphazero-shedding-new-light-grand-games-chess-shogi-and-go
  - GAN ? 
  - word2vec > Semi-surpervised Sequence learning > BERT > DistilBERT
1. transfer learning
  - style transfer, 
  - decrappification
1. machine learning and ethics
  - data and bias
  - visualization, disentanglement, interpretability
  - 



## Basics

* AI > **machine learning** > deep learning
![word cloud](https://iiot-world.com/wp-content/uploads/2017/05/word-cloud.png)
![https://towardsdatascience.com/rolling-in-the-deep-learning-basic-concepts-for-everyone-84bdb4766d18](https://miro.medium.com/max/1107/0*YQsvWvbnIW8OBQVT)
  ???: machine learning is the practice of algorthims to findi patterns in data
  * computer vision
  * natural language 
  
* types of learning
	> [https://machinelearningmastery.com/types-of-learning-in-machine-learning/](https://machinelearningmastery.com/types-of-learning-in-machine-learning/)

* tensors: life in n-dimensions 

* deep learning models:
  * feed-forward
  * convolutional neural networks (CNN)
  ![CNN](https://miro.medium.com/max/1065/1*itcofCIVsGe7rBmciJcmVw.gif)
  * recurrent 
  ![rnn animation](https://miro.medium.com/max/964/1*xn5kA92_J5KLaKcP7BMRLA.gif)
    * see: https://towardsdatascience.com/animated-rnn-lstm-and-gru-ef124d06cf45
    * RNN > LSTM > Attention networks
  * variational auto-encoders (VAE)
  * reinforcement learning (RL)
  * generative adversarial networks (GAN)

* pre-trained models:  
  ImageNet (from tf.keras.applications)
    Xception
    VGG16, VGG19
    ResNet, ResNetV2
    InceptionV3
    InceptionResNetV2
    MobileNet, MobileNetV2
    DenseNet
    NASNet
  NLP:
    Semi-supervised Sequence Learning, Generative Pre-Training, ELMo, and ULMFit 
    Bert, (Bi-directional):
      see: https://github.com/google-research/bert#what-is-bert
      > Input: the man went to the [MASK1] . he bought a [MASK2] of milk.
      > Labels: [MASK1] = store; [MASK2] = gallon    

* transfer learning



### lifecycle
* dataset
* train/validate
* test
* deploy





### concepts
1. data, data, data
  * the AI revolution: powered by data and processing
  * AI > machine learning > deep learning
  > see: https://becominghuman.ai/connection-between-data-science-ml-and-ai-d1c18d89b0bd
1. predictions and probability
  * regression vs classification
1. what is it good for?
  * computer vision
  * natural language, 
    * translation, auto-correct, grammarly, 
  * collaborative filtering, recommender systems
  * reinforcement learning
  * generative adversarial networks
  * self-driving cars
  * popular pretrained models
1. whats under the covers?
  * logistic neurons
  * loss equations
  * optimization with back-propagation and gradient descent
  * train/validate/test
  * benchmarks
1. how does it really work?
  * data preprocessing, everything is a number
  * train/validate/test
  * feature visualization and disentanglement
  * deploy
  * transfer learning
1. how much is a lot?
  * how many "variables" is enough?
    * how much is 1 quadrillion?
  * living in n-dimensional space
    * dimensionality reduction: projections to 2,3 dimensions
1. learn a lot, but not too much
  * bias and variance, over-fitting
1. how smart is smart?
  * human accuracy  
1. do more, quickly, with transfer learning  
  * pre-trained models

1. ethics
  * garbage in, garbage out
  * Moral Machines



* supervised vs un-supervised learning
* regression vs. classification
  * prediction vs probability
* neural networks
  * logistic neuron
  * hidden layers
  * how many parameters?


![ImageNet pre-trained models by parameters sorted by accuracy](https://i.postimg.cc/BvMz6Dbj/Screen-Shot-2019-12-06-at-9-47-32-AM.png)](https://postimg.cc/B8Pp7jx3)


* datasets: 
  * everything is a number
  * train/validation/test
* deep learning networks
  * n-dimensional space
* loss equations
> netowrks & loss equations in real life: what's the derivative of dx/dy? 
>   test/open book test/internet ok/ask siri
* optimizing with Gradient Descent
  * backpropagation
* bias vs. variance
  * overfitting, regularization
* pre-trained models & transfer learning
  * IMPORTANT!!!
* predictions

* optimizing loss equations with gradient descent
![gradient descent](https://easyai.tech/wp-content/uploads/2019/01/tiduxiajiang-1.png)



## deep learning IRL
__Multiple Choice Test__
1. whats the derivative of y=2x^3?     [] 3x^2          [] 2x^2           [x] 6x^2
1. what is the graph of y=-2x^2        []               [x]               [] 
1. what is 0/0?                        [x] indeterminate [] 0             [] infinity

loss equation: how many wrong? x/3
back propagation: change answer to get fewer wrong 
higher capacity models: test, study first, open book test, use internet, ask siri
over-fitting: diagonal

## Colab Notebooks
What does the network see? [https://distill.pub/2018/building-blocks/](https://distill.pub/2018/building-blocks/)
> how	activations at different layers influence decisions

## Quotes
[back to top](#toc)
> "Just as electricity transformed almost everything 100 years ago, today I actually have a hard time thinking of an industry that I don’t think AI will transform in the next several years." –Andrew Ng, Google Brain, Baidu, Coursera

> "Pretty much anything that a normal person can do in <1 sec, we can now automate with AI." –Andrew Ng

## Interesting
[back to top](#toc)
* visualizations and disentanglement, 
  * https://distill.pub/2017/feature-visualization/


![computer vision](https://s3-ap-south-1.amazonaws.com/av-blog-media/wp-content/uploads/2017/08/08131743/temp5.png)
10 Advanced Deep Learning Architectures Data Scientists Should Know!
> see:https://www.analyticsvidhya.com/blog/2017/08/10-advanced-deep-learning-architectures-data-scientists/

Understanding LSTM Networks
> see: http://colah.github.io/posts/2015-08-Understanding-LSTMs/

The fall of RNN / LSTM
> see: https://towardsdatascience.com/the-fall-of-rnn-lstm-2d1594c74ce0

Google’s Neural Machine Translation System
> see: http://tsong.me/blog/google-nmt/

Bert
  ![distilBert](https://miro.medium.com/max/2070/1*IFVX74cEe8U5D1GveL1uZA.png)
Hugging Face

**adversarial attacks**
see: [https://distill.pub/2019/activation-atlas/](https://distill.pub/2019/activation-atlas/)
![probability](https://i.postimg.cc/Hxf0nYSr/shark-or-baseball.png)

see: https://medium.com/syncedreview/adversarial-patch-on-hat-fools-sota-facial-recognition-82e8c4f83498
![enter image description here](https://miro.medium.com/max/1294/0*YCd7eIfFBoe2BewB.png)

perceptrons are like atoms
- combine the same atoms to get different people (1e27)
- combine perceptrons in different ways to get different models (1e9)

Where does data come from?
- #tenYearChallenge

## Headlines
### medical imaging
	# Google details AI that classifies chest X-rays with human-level accuracy
	# DeepMind’s AI can recommend treatment for more than 50 eye diseases with 94% accuracy
	# Google’s DeepMind wants AI to spot kidney injuries
	# Baidu Research’s breast cancer detection algorithm outperforms human pathologists
### jobs

### AI beats humans at



## Ethics and Issues 
[back to top](#toc)
> limitations: [https://towardsdatascience.com/the-limitations-of-machine-learning-a00e0c3040c6](https://towardsdatascience.com/the-limitations-of-machine-learning-a00e0c3040c6)

* bias
* skynet
* universal basic income
* rethinking education

![moral machines](https://media.nature.com/w800/magazine-assets/d41586-018-07135-0/d41586-018-07135-0_16219594.png)
see: https://www.nature.com/articles/d41586-018-07135-0
![who should die](https://s3-eu-west-1.amazonaws.com/elasticbeanstalk-eu-west-1-981246043789/wp-content/uploads/2018/08/13152336/Different-scenarios-of-a-self-driving-car-s-behavior-on-the-road.jpg)

## Glossary
[back to top](#toc)
* machine learning
* data science
* artificial intelligence
* petaflop/s-day: 1e15 ops/sec * ~1e5 secs, or 8.6e19 ops. AlphaGo trained on 1860 pf/s-d
* transfer learning - a machine learning algo is trained in 2 steps, 1) general training on a benchmark data set, followed by 2) fine-tuning on a smaller dataset to learn a specific target task. based on the principle that general features can be reused to learn specific tasks


# useful
> reverse image search, https://tineye.com

![Imagenet](https://4.bp.blogspot.com/-9jVHM1Pcsx8/WWUJxfwGTgI/AAAAAAAAB3k/-yLJh8EQQCUXqobeEfob49ekBBjLqQ0JgCLcBGAs/s1600/image1.png)

Computation required for inference with some of the largest deep learning models

Computation required for training some of the largest deep learning models
![Ai is changine the entire nature of compute](https://www.igrc.eu/wp-content/uploads/2019/06/ai-is-changing-the-entire-nature-of-compute-800x445.png)
https://www.igrc.eu/news/ai-is-changing-the-entire-nature-of-compute/


# from code
* computers are making decisions that affect your daily life
  * newsfeed,
  * advertising
  * face detection, image recognition, snapchat filters, photography: low-light, portrait mode, Face ID
  * language translation, spell/grammar check, alexa/siri/hey google
  * self-driving cars
* ML is how computers recognize patterns and make decisions by learning on data
  * learning comes from data, any kind of data that can be reduced to numbers
  * recognizing patterns in data and make predictions based on patterns
training data
  * train with bad data means bad decisions
  * where does data come from?
  * biased data favor some features (whether intentional or not) and ignore others
* impact on society
  * 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM3OTM0NTgzMywtMTIzMjcwMTIyMCw2Nj
IwNDk5OTEsMjE4NjE3MzA3LC01NTE1Mzc5MzcsLTE2Njk0OTYy
NDIsMjI2NTEyMTAwLC00MzU2NTU3NDIsLTE5MTQ5MzYwMTQsMT
U4NTkxMTAwLDY3Mjc5NzI4Myw5OTkxNjMwNTQsMjA5Mjc3MzI3
MiwtODY1NTcxMDcsLTI3MjQ5NjExNSwxNTk2NjY1NTY2LDMzND
AwNzcxMl19
-->