```
- diagram a perceptron
- 
```

## Classification Challenge: predict blue or orange dots found in a 2D space
> “Pretty much anything that a normal person can do in <1 sec, we can now automate with AI.” –Andrew Ng
### Man vs Machine
Predict blue or orange dots after viewing a sample of the data:
-	**Humans:** draw a line to separate blue/orange; make predictions
-	**AI:** learn a model from training data to predict blue or orange
	
## TF Playground Overview
1. Data (Classification)
	- 2-class dataset, blue/orange
	- randomly generated in 2D using different mathematical functions
	> click `regenerate` to show different samples					
	- separated into train and test data: you can look at the training set, but your predictions are evaluated on the test set
	
			NOTE: for fullscreen view of raw data, see Output Panel with output layer weights=0
			TODO: get fullscreen projection of data for human challenge
	
2. Neural Network/Model
	- basic building block is the perceptron,  
	- networks/models are built by connecting perceptrons in creative ways. 
	- there are many valid solutions; it's an art not a science, 

3. Features (Inputs)
> predict blue/orange dots on a 2D chart based on a sample from the dataset.
![circle](https://i.postimg.cc/cHqGVcW3/tfp-data1.png)

![XOR](https://i.postimg.cc/25LfcKsm/tfp-data2.png)
![???](https://i.postimg.cc/cHQGZ81b/tfp-data3.png)
![spiral](https://i.postimg.cc/SRkFKNJN/tfp-data4.png)
	- raw data: x1, x2  or `(x,y)`
	- "feature engineering" is the manipulation of raw data to create useful features for learning, access to 5 additional engineered features, e.g. x1^2 , x2*x2.
	
4. Hidden Layers
	- this is where you get the big money
	- build models in 2D, wide & deep, 
	- this is the "deep" in "deep learning"
			
			???: what is the relationship between number of perceptrons and n-dimensions of hyperplane
			
5. Output Layer: make predictions
	- for classification challenges: predictions expressed as a probability

## Learning
1. Loss functions: e.g. `% wrong`
2. Gradient Descent: learn the parameters which produce the lowest loss

		TODO: show animation of gradient descent
4. train vs test set

## Scoring/Evaluation
How do you know who  "won" or which model is "best"
1. compare accuracy
	- test loss, expressed as `% wrong`
	- color intensity shows confidence in prediction, 100% is the darkest
	- **regularization** to improve accuracy on test data
2. compare resources used:
	3. how long it took to "learn"
		- **model** determines the "terrain" of the loss surface
		- **learning rate, activation function, optimization function** determine the path you take to reach the "bottom"
	5. how long it takes to make a prediction, e.g. **inference**
		- proportional to how many parameters in your model



> Written with [StackEdit](https://stackedit.io/).

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbNTIwOTc5NDcsMTY3NzE1NzY1NiwtNDM3Mj
M4MjQ3XX0=
-->