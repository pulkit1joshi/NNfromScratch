# NNfromScratch - Neural Network From Scratch
We all use tensorflow , keras , for making convolution layers , dense layers , activations etc. Often people are not sure about what is going in the back , what is the mathematics behind it and how it is implemented. So I have tried to implement Neural Network from scratch and ran it on MNIST dataset. 

### Libraries :
Following libraries were used to build the NN from scratch
1. numpy : Neural Network is implemented using Numpy only.
2. matplotlib : Used to view the accuracy of MNIST dataset.
3. google colab : Trained it using google colab. One may train it on local machine aswell.

## Explaination
The whole concept can be divided as:
1.Layer 
2.Relu
3.DenseLayer
4.Lossfunction
5.GradientofLossFunction

### How NN Works?
1. First we initialize random weights in each layer.
2. Forward propagation of input takes place. Suppose first dense layer is **f(X) = WX + B** and second is (here) Relu. So after relu we get max(f(X),0) as the result.Similiarly, here we have built three dense layers and two relus.
3. Activations array will store results after every layer. So activation[0] corresponds to results after dense layer 1
4. Now as the input travels to the end we get **y'**. Now we canculate error. Here we have used Xentropy as error.
5. Now we backpropagate as suppose L is loss then , dL/dW1 and dl/dW2 are gradient to last nodes(if two) , then one may get other dl/dWs using chain rule.

### to be continued

### Accuracy 
* Blue - Training accuracy
* Orange - Validation accuracy
 
![Accuracy Graph](https://github.com/tobehonest/NNfromScratch/blob/master/Accuracy%20graph.png)

### TO DO LIST
1. Add better weights initializations
2. Regularisation
3. Image scrapper for extracting numbers from google


