**Prereqs**
```
- explore diagram of a perceptron, including: weights, bias, activation
- show examples of how perceptrons can be connected together
	- show pretrained models
???: loss functions & gradient descent?
???: train/test workflow?
???: the power of n-dimensions & overfitting
???: evaluating/comparing models

```




## Classification Challenge: predict blue or orange dots found in a 2D space
> “Pretty much anything that a normal person can do in <1 sec, we can now automate with AI.” –Andrew Ng
### Man vs Machine
Predict blue or orange dots on a 2D chart from a sample of the dataset:
-	**Humans:** draw a line to separate blue/orange; make predictions
-	**AI:** learn a model from training data to predict blue or orange
	
## TF Playground Overview
1. Data (Classification)
![data](https://i.postimg.cc/t4qm8psS/tf-playground-data.png =240x240)
	- 2-class dataset, blue/orange
	- randomly generated in 2D using different mathematical functions
	> click `regenerate` to show different samples					
	- separated into train and test data: you can look at the training set, but your predictions are evaluated on the test set
	> predict blue/orange dots on a 2D chart based on a sample from the dataset.
![circle](https://i.postimg.cc/cHqGVcW3/tfp-data1.png)

![XOR](https://i.postimg.cc/25LfcKsm/tfp-data2.png)
![???](https://i.postimg.cc/cHQGZ81b/tfp-data3.png)
![spiral](https://i.postimg.cc/SRkFKNJN/tfp-data4.png)

	
2. Neural Network/Model
	- basic building block is the perceptron,  
	- networks/models are built by connecting perceptrons in creative ways. 
	- there are many valid solutions; it's an art not a science, 

3. Features (Inputs)
![features](https://i.postimg.cc/Mp9rSNRW/tf-playground-features.png =240x240)
	- raw data: x1, x2  or `(x,y) coordinates for each orange/blue dot`
	- "feature engineering" is the manipulation of raw data to create useful features for learning, access to 5 additional engineered features, e.g. x1^2 , x2*x2.
	
4. Hidden Layers
![network](https://i.postimg.cc/CKdrL7Hb/rf-playground-network.png =240x240)
	- built by connecting many perceptrons in creative ways
	- build models in 2D, wide & deep. This is the "deep" in "deep learning"
	- explain activations
			
			???: what is the relationship between number of perceptrons and n-dimensions of hyperplane
			
5. Output Layer: convert final activations into predictions
![output](https://i.postimg.cc/tgfS162w/tf-playground-ouput.png =240x240)
	- for classification challenges: predictions expressed as a probability

## Learning
![train](https://i.postimg.cc/zX1QSn81/tf-playground-train.png =240x240)
1. Loss functions: e.g. `% wrong`
2. Gradient Descent: learn the parameters which produce the lowest loss

		TODO: show animation of gradient descent
4. train vs test set

## Compare/Score/Evaluate
![inference](https://i.postimg.cc/1tqWDzdt/tf-playground-predict.png =240x240)
How do you know who  "won" or which model is "best"?

### accuracy
	- test loss, expressed as `% wrong`
	- color intensity shows confidence in prediction, 100% is the darkest
	- color intensity between the neurons proportional to learned weights
1. **overfitting**
![overfitting](https://i.postimg.cc/zGsS5pnf/tfp-overfitting.png)
	- [https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=xor&regDataset=reg-plane&learningRate=0.03&regularizationRate=0.03&noise=30&networkShape=8,8,8,8,8&seed=0.35842&showTestData=false&discretize=false&percTrainData=20&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false](https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=xor&regDataset=reg-plane&learningRate=0.03&regularizationRate=0.03&noise=30&networkShape=8,8,8,8,8&seed=0.35842&showTestData=false&discretize=false&percTrainData=20&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false)
	> Note: when the intensity of connections between neurons is darker, suggesting that the input strongs

	
2. **regularization**: improve accuracy on test data by preventing the network from "learning" too much(!)
![regularization](https://i.postimg.cc/85DRf5XQ/tfp-regularization.png)
	
	
4. compare resources used:
	3. how long it took to "learn"
		- **model** determines the "terrain" of the loss surface
		- **learning rate, activation function, optimization function** determine the path you take to reach the "bottom"
	5. how long it takes to make a prediction, e.g. **inference**
		- proportional to how many parameters in your model


> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4Njk5NjE5NTgsLTUxMzY4MDQ3NSwtMT
k4MDkyNjcxNSwtOTQ1Mzg3MzkzLDE2NzcxNTc2NTYsLTQzNzIz
ODI0N119
-->