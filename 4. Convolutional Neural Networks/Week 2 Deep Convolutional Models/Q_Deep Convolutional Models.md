# Quiz

1. Which of the following do you typically see in a ConvNet? (Check all that apply.)
    - Multiple CONV layers followed by a POOL layer
    - FC layers in the last few layers
    
2. In order to be able to build very deep networks, we usually only use pooling layers to downsize the height/width of the activation volumes while convolutions are used with “valid” padding. Otherwise, we would downsize the input of the model too quickly.
    - False
    
3. Training a deeper network (for example, adding additional layers to the network) allows the network to fit more complex functions and thus almost always results in lower training error. For this question, assume we’re referring to “plain” networks.
    - False
    
4. The following equation captures the computation in a ResNet block. What goes into the two blanks above?
    
    ![Untitled](Quiz%206026a6b1ffbf453789113ef88261b83d/Untitled.png)
    
    - $a^{[l]} and \ 0, respectively$
    
5. Which ones of the following statements on Residual Networks are true? (Check all that apply.)
    - The skip-connection makes it easy for the network to learn an identity mapping between the input and the output within the ResNet block.
    - Using a skip-connection helps the gradient to backpropagate and thus helps you to train deeper networks
    
6. Suppose you have an input volume of dimension  $n_H \times n_W \times n_C$. Which of the following statements you agree with? (Assume that “1x1 convolutional layer” below always uses a stride of 1 and no padding.)
    - You can use a 1x1 convolutional layer to reduce $n_C$ but not $n_H$, $n_W$.
    - You can use a 2D pooling layer to reduce $n_H$, $n_W$ but not n_C.
    
7. Which ones of the following statements on Inception Networks are true? (Check all that apply.)
    - A single inception block allows the network to use a combination of 1x1, 3x3, 5x5 convolutions and pooling.
    - Inception blocks usually use 1x1 convolutions to reduce the input data volume’s size before applying 3x3 and 5x5 convolutions.
    
8. Which of the following are common reasons for using open-source implementations of ConvNets (both the model and/or weights)? Check all that apply.
    - Parameters trained for one computer vision task are often useful as pretraining for other computer vision tasks.
    - It is a convenient way to get working with an implementation of a complex ConvNet architecture.
    
9. In Depthwise Separable Convolution you:
    - Perform two steps of convolution.
    - You convolve the input image with $n_c$ number of $n_f \times n_f$ filters ($*n_c$ is the number of color channels of the input image*).
    - The final output is of the dimension  $n_{out} \times n_{out} \times n^{'}_{c}$(*where $n^{'}_{c}$ is the number of filters used in the previous convolution step*).
    - For the “Depthwise” computations each filter convolves with only one corresponding color channel of the input image.
    
10. Fill in the missing dimensions shown in the image below (*marked W, Y, Z*).
    
    ![Untitled](Quiz%206026a6b1ffbf453789113ef88261b83d/Untitled%201.png)
    
    - W = 5, Y = 30, Z = 20