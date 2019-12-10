# outline
1. AI > machine learning > deep learning
	- machines are making decisions using "A.I." that affect you every day, examples:
		- **today:** social media feeds, snapchat filters, Siri/Alexa, Google Translate, Portrait mode, Face ID, recommender engines, online advertising, grammarly
		- **tomorrow:** self-driving cars, medicine

![ai beats humans](https://i.ibb.co/4sdFz9L/Screenshot-2019-12-10-at-11-53-15-AM.png)

2. What is it?
	CS: tell a computer what to do by programming it step-by-step
	ML: teach a computer to make predictions by learning hidden patterns in data
	
		> decision: action based on predictions
		
3. What does that looks like?

> show example of inference


> example of transfer learning, train on a dataset





4. How does this really work? (a simple example)

	* features: made of weights and bias
![perceptron](https://miro.medium.com/max/1435/1*n6sJ4yZQzwKL9wnF5wnVNg.png)	
	* millions of them hooked together
![animated CNN](https://miro.medium.com/max/1920/1*eEKb2RxREV6-MtLz2DNWFQ.gif)
	* what is actually learned? the model and the weights
	
> datasets + pre-trained models = transfer learning

		1. datasets and benchmarks
			* CiFAR, ImageNet
		2. pre-trained models and embeddings
			* image recognition
			* BERT, word2vec
			* RL
			* GANS
		3. transfer learning

> transfer learning IRL: closed book, open book, lifeline, hey siri

5. Behind the curtain (more detail)
	* **learning lifecycle:** train/validate/test/deploy
	* supervised vs. unsupervised learning 
	* everything is a number
	* predictions are probabilities
	* loss equations determine what is learned
	* learning with gradient descent
![gradient descent](https://easyai.tech/wp-content/uploads/2019/01/tiduxiajiang-1.png)
	* metrics
	* deployment & inference

6. Why does this work? 
	* life in n-dimensions
		* **bias**: predictions made without considering all the patterns hidden in the data
		* dimensionality reduction video
		* how much is a billion?
	* data, data, data
		* **variance**: how much predictions change as the data changes (over-fitting)
	* Petaflop/sec-day

7. What is Hiding in the Data?
	* what does the model see? 
		* What does the network see? 
![enter image description here](https://distill.pub/2018/building-blocks/examples/activations/dog_cat/mixed4d.jpeg)
		* [https://distill.pub/2018/building-blocks/](https://distill.pub/2018/building-blocks/)
		* shark vs baseball: [https://distill.pub/2019/activation-atlas/](https://distill.pub/2019/activation-atlas/)
		* clustering of semantic concepts [https://distill.pub/2019/activation-atlas/#focus-playground](https://distill.pub/2019/activation-atlas/#focus-playground)
	* word math with word2vec
	*  	

8. What did we really learn?
	* robust vs non-robust features
	* adversarial examples
	* attribution, disentanglement,  interpretability


9. different models for different tasks
	- feed forward
	- CNN
	- RL
	- GANS
	- RNN/LSTM/attention

10. How do you learn something useful?
	
	> ImageNet: learning breakthroughs by model architecture
	> model architecture and loss equations

11. It's an art, not a science
	- ImageNet breakthroughs
	- path of new ideas/breakthroughs

12. limitations: human error
	* [human level performance](https://towardsdatascience.com/how-to-improve-my-ml-algorithm-lessons-from-andrew-ngs-experience-ii-f66926926f88)

	 
13. limitations: ethics
	see: [limitations](https://towardsdatascience.com/the-limitations-of-machine-learning-a00e0c3040c6)
	* where does data come from?
	* bias in labeled datasets
	* bias in unsupervised learning
	* bad data means bad predictions
	* moral compass
> bias in datasets


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQxMDU3MDM4NywxOTI5NTU1NjMyLC03OD
I3NzMyMTQsNDI0OTgyMzA4LDI0NDM2NzYyNSwxNTUwNTQxNDAz
LC0xNjY5NzMyMDY3LC03MDU1MDI0MzEsODI5NjM2MjYyLDE4Nz
k0NzQ4NzksMTg3MzgzNjEyOSwxNjY2NjU5MTg2LC0xNDU1ODEw
OTM5LC0yNTgxMDM5NjcsLTE1MzQ5OTA2NDQsMjA0MDI5NzYyMl
19
-->