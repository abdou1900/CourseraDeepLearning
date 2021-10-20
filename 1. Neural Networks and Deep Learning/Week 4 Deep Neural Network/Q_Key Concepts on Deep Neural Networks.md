# Q_Key Concepts on Deep Neural Networks

1. What is the "cache" used for in our implementation of forward propagation and backward propagation?
    - [ ]  It is used to cache the intermediate values of the cost function during training.
    - [x]  We use it to pass variables computed during forward propagation to the corresponding backward propagation step. It contains useful values for backward propagation to compute derivatives.
    - [ ]  It is used to keep track of the hyperparameters that we are searching over, to speed up computation.
    - [ ]  We use it to pass variables computed during backward propagation to the corresponding forward propagation step. It contains useful values for forward propagation to compute activations.
    
    > the "cache" records values from the forward propagation units and sends it to the backward propagation units because it is needed to compute the chain rule derivatives.
    > 
    
2. Among the following, which ones are "hyperparameters"? (Check all that apply.)
    - size of the hidden layers n^[l]
    - learning rate α
    - number of iterations
    - number of layers L in the neural network
    
3. Which of the following statements is true?
    - [x]  The deeper layers of a neural network are typically computing more complex features of the input than the earlier layers. Correct
    - [ ]  The earlier layers of a neural network are typically computing more complex features of the input than the deeper layers.
    
4. Vectorization allows you to compute forward propagation in an L-layer neural network without an explicit for-loop (or any other explicit iterative loop) over the layers l=1, 2, …,L. True/False?
    - [ ]  True
    - [x]  False
    
    Note: We cannot avoid the for-loop iteration over the computations among layers.
    
5. Assume we store the values for n^[l] in an array called layers, as follows: layer_dims = [n_x, 4,3,2,1]. So layer 1 has four hidden units, layer 2 has 3 hidden units and so on. Which of the following for-loops will allow you to initialize the parameters for the model?
    
    ![Untitled](Q_Key%20Concepts%20on%20Deep%20Neural%20Networks%203c5595066ae14c7e821e43b1e107ee52/Untitled.png)
    
6. Consider the following neural network.
    - The number of layers L is 4. The number of hidden layers is 3.
    
    Note: The input layer (L^[0]) does not count.
    
    > As seen in lecture, the number of layers is counted as the number of hidden layers + 1. The input and output layers are not counted as hidden layers.
    > 
    
7. During forward propagation, in the forward function for a layer l you need to know what is the activation function in a layer (Sigmoid, tanh, ReLU, etc.). During backpropagation, the corresponding backward function also needs to know what is the activation function for layer l, since the gradient depends on it. True/False?
    - [x]  True
    - [ ]  False
    
    > During backpropagation you need to know which activation was used in the forward propagation to be able to compute the correct derivative.
    > 
    
8. There are certain functions with the following properties:
    
    (i) To compute the function using a shallow network circuit, you will need a large network (where we measure size by the number of logic gates in the network), but (ii) To compute it using a deep network circuit, you need only an exponentially smaller network. True/False?
    
    - [x]  True
    - [ ]  False
    
9. Consider the following 2 hidden layer neural network:
    
    ![Untitled](Q_Key%20Concepts%20on%20Deep%20Neural%20Networks%203c5595066ae14c7e821e43b1e107ee52/Untitled%201.png)
    
    Which of the following statements are True? (Check all that apply).
    
    - W^[1] will have shape (4, 4)
    - b^[1] will have shape (4, 1)
    - W^[2] will have shape (3, 4)
    - b^[2] will have shape (3, 1)
    - b^[3] will have shape (1, 1)
    - W^[3] will have shape (1, 3)
    
10. Whereas the previous question used a specific network, in the general case what is the dimension of W^[l], the weight matrix associated with layer l?
    - W^[l] has shape (n^[l],n^[l−1])