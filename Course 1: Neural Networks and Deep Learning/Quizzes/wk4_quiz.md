### Week 4 Quiz - Key concepts on Deep Neural Networks

1. Question 1
What is the "cache" used for in our implementation of forward propagation and backward propagation?

    [x] We use it to pass variables computed during forward propagation to the corresponding backward propagation step. It contains useful values for backward propagation to compute derivatives.

2. Question 2
Among the following, which ones are "hyperparameters"? (Check all that apply.)

    [x] number of layers L in the neural network
    [x] size of the hidden layers n^[l]
    [x] learning rate α
    [x] number of iterations    

3. Question 3
Which of the following statements is true?

    [x] The deeper layers of a neural network are typically computing more complex features of the input than the earlier layers.

4. Question 4
Vectorization allows you to compute forward propagation in an L-layer neural network without an explicit for-loop (or any other explicit iterative loop) over the layers l=1, 2, …,L. True/False?

    [x] False
    
    Note: We cannot avoid the for-loop iteration over the computations among layers.

5. Question 5
Assume we store the values for n^[l] in an array called layers, as follows: layer_dims = [n_x, 4,3,2,1]. So layer 1 has four hidden units, layer 2 has 3 hidden units and so on. Which of the following for-loops will allow you to initialize the parameters for the model?

    [x] ```for(i in range(1, len(layer_dims))):
                parameter[‘W’ + str(i)] = np.random.randn(layers[i], layers[i - 1])) * 0.01
                parameter[‘b’ + str(i)] = np.random.randn(layers[i], 1) * 0.01
        ```

6. Question 6    
Consider the following neural network.

How many layers does this network have?

    [x] The number of layers L is 4. The number of hidden layers is 3.

7. Question 7        
During forward propagation, in the forward function for a layer l you need to know what is the activation function in a layer (Sigmoid, tanh, ReLU, etc.). During backpropagation, the corresponding backward function also needs to know what is the activation function for layer l, since the gradient depends on it. True/False?

    [x] True

8. Question 8        
There are certain functions with the following properties:

(i) To compute the function using a shallow network circuit, you will need a large network (where we measure size by the number of logic gates in the network), but (ii) To compute it using a deep network circuit, you need only an exponentially smaller network. True/False?
    
    [x] True

9. Question 9        
Consider the following 2 hidden layer neural network:

    Which of the following statements are True? (Check all that apply).

    [x] W^[1] will have shape (4, 4)
    [x] b^[1] will have shape (4, 1)
    [x] W^[2] will have shape (3, 4)
    [x] b^[2] will have shape (3, 1)    
    [x] W^[3] will have shape (1, 3)
    [x] b^[3] will have shape (1, 1)
    
    Note: See [this image](https://user-images.githubusercontent.com/14886380/29200515-7fdd1548-7e88-11e7-9d05-0878fe96bcfa.png) for general formulas.   

10. Question 10       
Whereas the previous question used a specific network, in the general case what is the dimension of W^[l], the weight matrix associated with layer l?

    [x] W^[l] has shape (n^[l],n^[l−1])
    
    Note: See [this image](https://user-images.githubusercontent.com/14886380/29200515-7fdd1548-7e88-11e7-9d05-0878fe96bcfa.png) for general formulas.