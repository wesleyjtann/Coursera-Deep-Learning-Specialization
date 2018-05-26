### Week 10 quiz - The basics of ConvNets

1. Question 1
What do you think applying this filter to a grayscale image will do?

	[x] Detect vertical edges

2. Question 2 
Suppose your input is a 300 by 300 color (RGB) image, and you are not using a convolutional network. If the first hidden layer has 100 neurons, each one fully connected to the input, how many parameters does this hidden layer have (including the bias parameters)?

	[x] `(300x300x3)x100+100 = 27,000,100`

3. Question 3
Suppose your input is a 300 by 300 color (RGB) image, and you use a convolutional layer with 100 filters that are each 5x5. How many parameters does this hidden layer have (including the bias parameters)?

	[x] `(5x5x3)x100+100 = 7600`

4. Question 4
You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, using a stride of 2 and no padding. What is the output volume?
	
	Using formula `(n+2p-f)/2 + 1`
	[x] 29x29x32

5. Question 5  
You have an input volume that is 15x15x8, and pad it using “pad=2.” What is the dimension of the resulting volume (after padding)?

	[x] 19x19x8

6. Question 6    
You have an input volume that is 63x63x16, and convolve it with 32 filters that are each 7x7, and stride of 1. You want to use a “same” convolution. What is the padding?
	
	Using `floor((63+2p-7)/1) = 63`, solve for `p`.
	[x] 3

7. Question 7    
You have an input volume that is 32x32x16, and apply max pooling with a stride of 2 and a filter size of 2. What is the output volume?

	[x] 16x16x16

8. Question 8    
Because pooling layers do not have parameters, they do not affect the backpropagation (derivatives) calculation.

	[x] False

9. Question 9    
In lecture we talked about “parameter sharing” as a benefit of using convolutional networks. Which of the following statements about parameter sharing in ConvNets are true? (Check all that apply.)

	[x] It reduces the total number of parameters, thus reducing overfitting.
	[x] It allows a feature detector to be used in multiple locations throughout the whole input image/input volume.

10. Question 10    
In lecture we talked about “sparsity of connections” as a benefit of using convolutional layers. What does this mean?

	[x] Each activation in the next layer depends on only a small number of activations from the previous layer.
