### Week 11 quiz - Deep convolutional models

1. Question 1
Which of the following do you typically see as you move to deeper layers in a ConvNet?

	[x] nH and nW decrease, while nC increases

2. Question 2
Which of the following do you typically see in a ConvNet? (Check all that apply.)

	[x] Multiple CONV layers followed by a POOL layer
	[x] FC layers in the last few layers

3. Question 3
In order to be able to build very deep networks, we usually only use pooling layers to downsize the height/width of the activation volumes while convolutions are used with “valid” padding. Otherwise, we would downsize the input of the model too quickly.

	[x] False

4. Question 4
Training a deeper network (for example, adding additional layers to the network) allows the network to fit more complex functions and thus almost always results in lower training error. For this question, assume we’re referring to “plain” networks.

	[x] False

5. Question 5  
The following equation captures the computation in a ResNet block. What goes into the two blanks above?
```
a[l+2]=g(W[l+2]g(W[l+1]a[l]+b[l+1])+bl+2+_______ )+_______
```
	[x] a[l] and 0, respectively

6. Question 6    
Which ones of the following statements on Residual Networks are true? (Check all that apply.)

	[x] Using a skip-connection helps the gradient to backpropagate and thus helps you to train deeper networks
	[x] The skip-connection makes it easy for the network to learn an identity mapping between the input and the output within the ResNet block.

7. Question 7
Suppose you have an input volume of dimension 64x64x16. How many parameters would a single 1x1 convolutional filter have (including the bias)?

	[x] 17

8. Question 8  
Suppose you have an input volume of dimension nH x nW x nC. Which of the following statements you agree with? (Assume that “1x1 convolutional layer” below always uses a stride of 1 and no padding.)
	
	[x] You can use a pooling layer to reduce nH, nW, but not nC​. 
	[x] You can use a 1x1 convolutional layer to reduce nC but not nH, nW.

9. Question 9
Which ones of the following statements on Inception Networks are true? (Check all that apply.)

	[x] A single inception block allows the network to use a combination of 1x1, 3x3, 5x5 convolutions and pooling.
	[x] Inception blocks usually use 1x1 convolutions to reduce the input data volume’s size before applying 3x3 and 5x5 convolutions.

10. Question 10
Which of the following are common reasons for using open-source implementations of ConvNets (both the model and/or weights)? Check all that apply.

	[x] It is a convenient way to get working an implementation of a complex ConvNet architecture.
	[x] Parameters trained for one computer vision task are often useful as pretraining for other computer vision tasks.