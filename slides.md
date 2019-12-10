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

> show logistic neuron.  too much detail?

	* features: made of weights and bias
	* what is actually learned?
	
> datasets + pre-trained models = transfer learning

		1. datasets and benchmarks
			* CiFAR, ImageNet
		2. pre-trained models and embeddings
			* image recognition
			* BERT, word2vec
			* RL
			* GANS
		3. transfer learning

5. Behind the curtain (more detail)
	* **learning lifecycle:** train/validate/test/deploy
	* supervised vs. unsupervised learning 
	* everything is a number
	* loss equations determine what is learned
	* 
	* learning with gradient descent
![gradient descent](https://easyai.tech/wp-content/uploads/2019/01/tiduxiajiang-1.png)
	* 

6. Why does this work? 
	* life in n-dimensions
		* **bias**: predictions made without considering all the patterns hidden in the data
		* dimensionality reduction video
		* how much is a billion?
	* data, data, data
		* **variance**: how much predictions change as the data changes (over-fitting)
	* Petaflop/sec-day

7. What is Hiding in the Data, 
	* what does the model see? 
		* What does the network see? 
![enter image description here](https://distill.pub/2018/building-blocks/examples/activations/dog_cat/mixed4d.jpeg)
		* [https://distill.pub/2018/building-blocks/](https://distill.pub/2018/building-blocks/)
		* shark vs baseball: [https://distill.pub/2019/activation-atlas/](https://distill.pub/2019/activation-atlas/)
		* clustering of semantic concepts [https://distill.pub/2019/activation-atlas/#focus-playground](https://distill.pub/2019/activation-atlas/#focus-playground)
	* word math with word2vec
	*  	

8. different models for different tasks
	- feed forward
	- CNN
	- RL
	- GANS
	- RNN/LSTM/attention

9. how do you teach the right things?

> ImageNet: learning breakthroughs by model architecture
> model architecture and loss equations

9. It's an art, not a science
	- ImageNet breakthroughs
	- path of new ideas/breakthroughs

10. Adversarial Examples
11. ethics
	* where does data come from?
	* bias in labeled datasets
	* bias in unsupervised learning
	* bad data means bad predictions
	* moral compass
> bias in datasets


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM1MDY0MDE0LC0xNjY5NzMyMDY3LC03MD
U1MDI0MzEsODI5NjM2MjYyLDE4Nzk0NzQ4NzksMTg3MzgzNjEy
OSwxNjY2NjU5MTg2LC0xNDU1ODEwOTM5LC0yNTgxMDM5NjcsLT
E1MzQ5OTA2NDQsMjA0MDI5NzYyMl19
-->