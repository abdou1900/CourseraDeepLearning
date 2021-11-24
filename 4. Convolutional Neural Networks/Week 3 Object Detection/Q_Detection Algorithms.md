# Quiz

1. You are building a 3-class object classification and localization algorithm. The classes are: pedestrian (c=1), car (c=2), motorcycle (c=3). What should y*y* be for the image below? Remember that “?” means “don’t care”, which means that the neural network loss function won’t care what the neural network gives for that component of the output. Recall y = [$p_c, b_x, b_y, b_h, b_w, c_1, c_2, c_3$]
    
    ![Untitled](Quiz%20e82f236640db4307ae33aa3933ac7a64/Untitled.png)
    
    - y = [0, ?, ?, ?, ?, ?, ?, ?]
    
2. You are working on a factory automation task. Your system will see a can of soft-drink coming down a conveyor belt, and you want it to take a picture and decide whether (i) there is a soft-drink can in the image, and if so (ii) its bounding box. Since the soft-drink can is round, the bounding box is always square, and the soft drink can always appear as the same size in the image. There is at most one soft drink can in each image. Here’re some typical images in your training set:
    
    ![Untitled](Quiz%20e82f236640db4307ae33aa3933ac7a64/Untitled%201.png)
    
    What is the most appropriate set of output units for your neural network?
    
    - Logistic unit, $b_x$ and $b_y$
    
3. If you build a neural network that inputs a picture of a person’s face and outputs N landmarks on the face (assume the input image always contains exactly one face), how many output units will the network have?
    - 2N
    
4. When training one of the object detection systems described in lecture, you need a training set that contains many pictures of the object(s) you wish to detect. However, bounding boxes do not need to be provided in the training set, since the algorithm can learn to detect the objects by itself.
    - False
    
5. What is the IoU between these two boxes? The upper-left box is 2x2, and the lower-right box is 2x3. The overlapping region is 1x1.
    
    ![Untitled](Quiz%20e82f236640db4307ae33aa3933ac7a64/Untitled%202.png)
    
    - 1/9
    
6. Suppose you run non-max suppression on the predicted boxes above. The parameters you use for non-max suppression are that boxes with probability ≤ 0.4 are discarded, and the IoU threshold for deciding if two boxes overlap is 0.5. How many boxes will remain after non-max suppression?
    
    ![Untitled](Quiz%20e82f236640db4307ae33aa3933ac7a64/Untitled%203.png)
    
    - 5
    
7. Suppose you are using YOLO on a 19x19 grid, on a detection problem with 20 classes, and with 5 anchor boxes. During training, for each image you will need to construct an output volume y as the target value for the neural network; this corresponds to the last layer of the neural network. (y may include some “?”, or “don’t cares”). What is the dimension of this output volume?
    - 19x19x(5x25)
    
8. What is Semantic Segmentation?
    - Locating objects in an image by predicting each pixel as to which class it belongs to.
    
9. Using the concept of Transpose Convolution, fill in the values of **X**, **Y** and **Z** below. (*padding = 1, stride = 2*)
    
    ![Untitled](Quiz%20e82f236640db4307ae33aa3933ac7a64/Untitled%204.png)
    
    - X = 2, Y = -6, Z = -4
    
10. Suppose your input to an U-Net architecture is h*h* x w*w* x 33, where 3 denotes your number of channels (RGB). What will be the dimension of your output ?
    - h x w x n, where n = number of output classes