# Deep Neural Network

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/1_KHs1Chs6TCJDTIIQVyIJxg.png)

### Deep Neural Network
AI (Artificial Intelligence) covers many areas of research, from genetic algorithms to expert systems, and provides scope for arguments about what constitutes AI.

In the field of AI research, Machine Learning has enjoyed considerable success in recent years – allowing computers to surpass or come close to matching human performance in areas ranging from facial recognition to facial recognition. speech and language recognition.

Machine Learning is the process of teaching a computer to perform a task, instead of programming it how to perform that task step by step.

and Deep learning is derived from the Neural network algorithm, which comes from just a small branch of machine learning. Deep Learning is a branch of machine learning that relies on a set of algorithms to attempt to model highly abstracted data using multiple processing layers with complex structures, or otherwise including many nonlinear transformations.

It allows us to train an AI that can predict outputs based on a set of inputs. Both supervised and unsupervised methods can be used for training.

At the end of training, a Machine Learning system should be able to make accurate predictions when given the data.

### Machine Learning - Deep Neural Network Model
1. The brain of this predictive AI has neurons. These neurons are represented by circles and these circles are connected to each other.

     These neurons are grouped into 3 different layer types:

    Layer Input
    Layer(s) Hidden
    Layer Output

    The input layer receives input data. In this case, we have 11 neurons in the input layer. The input layer takes these inputs to the first hidden layer.

    The hidden layers perform mathematical calculations based on our output. One of the challenges when creating neural networks is deciding the number of hidden layers and the number of neurons for each layer.

    The output layer returns a data output which in this case is a prediction of the patient's condition for breast cancer

    Each connection between neurons is associated with a weight. This weight represents the importance of the input value. The initial weights are set at random (we call it Dummy Weight).

2. Each neuron has 1 Activation Function. and in this project I use sigmoid function as the activation function.
    + $a = \phi(z) = \frac{1}{1+e^{-z}}$
    + And its derivative: 
       + $\frac{\partial \sigma(x)}{\partial x} = \frac{e^{-x}}{(1+e^{-x})^2}$
 
    To train the model, we roughly feed it the inputs from the data set, and compare its outputs with the outputs from the data set. Since the model is still untrained, its output will be wrong.

    Once we have looked at the entire data set, we can create a cost function to show how the model outputs differed from the actual outputs. and I use mean square error as a cost function: 
    + $C_{(w, b)} = \frac {1} {n} \displaystyle\sum_{i=1}^N (Y_i - \hat{Y}_i)^2$


3. And the last step is to build a Dense Neural Network model. 

    Note: In each of layer in each network has two phase: Pre_activation phase and post_activation phase
    * pre_activation: This phase consist of weight linear combination of post_activation value of previous layer 
        * $\mathbf{z}^{\ell} = W^{\ell}\mathbf{a}^{\ell-1} + \mathbf{b}^{\ell},$ 
    * post_activation: This phase consist of passsing the pre_activation value through an activation function
        * $\mathbf{a}^{\ell} = \sigma(\mathbf{z}^{\ell}).$
  
4. After running the data and training model, the weights between neurons are adjusted by minimizing the cost function, you need to iterate over the data sets many times. That's why you need an amount of computational power.

     Updating weights with mean square error will be done automatically.

5. Then we can predict how well the model work on the test data, Compute the classification accuracy of our trained model and visualuze the mean suqare error over the training process