# Quiz

1. A Transformer Network, like its predecessors RNNs, GRUs and LSTMs, can process information one word at a time. (Sequential architecture).
    - False
    
2. Transformer Network methodology is taken from: (Check all that apply)
    - Attention mechanism.
    - Convolutional Neural Network style of processing.

1. The concept of *Self-Attention* is that:
    
    ![Untitled](Quiz%206736867f36bb4ac088d5ed3233a0a77f/Untitled.png)
    
    - Given a word, its neighbouring words are used to compute its context by summing up the word values to map the Attention related to that given word.

1. Which of the following correctly represents *Attention ?*
    - $Attention(Q, K, V) = softmax(\frac{QK^T}{\sqrt{d_k}})V$

1. Are the following statements true regarding Query (Q), Key (K) and Value (V) ?
    
    Q = interesting questions about the words in a sentence
    
    K = specific representations of words given a Q
    
    V = qualities of words given a Q
    
    - False

1. *i* here represents the computed attention weight matrix associated with the ith*ith* “word” in a sentence.
    
    ![Untitled](Quiz%206736867f36bb4ac088d5ed3233a0a77f/Untitled%201.png)
    
    - False
    
2. Following is the architecture within a Transformer Network. ***(without displaying positional encoding and output layers(s))***
    
    ![Untitled](Quiz%206736867f36bb4ac088d5ed3233a0a77f/Untitled%202.png)
    
    What information does the *Decoder* take from the *Encoder* for its second block of *Multi-Head Attention* ? (Marked X, pointed by the independent arrow) (Check all that apply)
    
    - K
    - V

1. Following is the architecture within a Transformer Network. ***(without displaying positional encoding and output layers(s))***
    
    ![Untitled](Quiz%206736867f36bb4ac088d5ed3233a0a77f/Untitled%203.png)
    
    What is the output layer(s) of the *Decoder* ? (Marked Y*Y*, pointed by the independent arrow)
    
    - Linear layer followed by a softmax layer.

1. Why is positional encoding important in the translation process? (Check all that apply)
    - Position and word order are essential in sentence construction of any language.
    - Providing extra information to our model.

1. Which of these is a good criteria for a good positionial encoding algorithm?
    - It should output a unique encoding for each time-step (word’s position in a sentence).
    - Distance between any two time-steps should be consistent for all sentence lengths.
    - The algorithm should be able to generalize to longer sentences.