# MaliciousURLDetectorUsingAutoencoder

Idea:
The idea is to employ deep learning method (autoencoder) to build a URLs classification model, which will be trained on normal (non malicious) URLs dataset. The resulting classifier will be able to distinguish between a malicious and a non malicious URL. 

How it works:
Using a training set of just legitimate transactions, we teach a machine learning algorithm to reproduce the feature vector of each transaction. Then we perform a reality check on such a reproduction. If the distance between the original transaction and the reproduced transaction is below a given threshold, the transaction is considered legitimate; otherwise it is considered a fraud candidate.

Autoencoder:
An autoencoder is a feed-forward multilayer neural network that reproduces the input data on the output layer. So, the number of output units must be the same as the number of input units. The autoencoder is here trained using the backpropagation algorithm againstthe mean squared error (MSE) loss function.

Implementation:
The implementation is coded in Python using Keras for building and training the model and Panda for data manipulation.
The dataet couldn't have been used in its original state, so some feature engineering has been done to make it more rich with new features engineered. 
