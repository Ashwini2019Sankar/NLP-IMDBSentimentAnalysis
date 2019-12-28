# NLP-IMDBSentimentAnalysis

Model summary : I have used the following layers in order -
Embedding layer(build my own)
Conv1D layer
Global Max Pooling
Dropout
Dense/Full connection layer

Optimization is a process of searching for parameters that minimize or maximize our functions.
When we train machine learning model, we usually use indirect optimization.

Adam : is an optimization algorithm that can be used instead of the classical SGD procedure to
update network weights iterative based on training data.

The optimizer used in my model is : ‘Adam’ & loss function used is : ‘binary_crossentropy’.

Binary Cross-entropy loss, or log loss, measures the performance of a classification model
whose output is a probability value between 0 and 1. Cross-entropy loss increases as the
predicted probability diverges from the actual label. So predicting a probability of .012 when the
actual observation label is 1 would be bad and result in a high loss value. A perfect model would
have a log loss of 0.

Model accuracy summary : At epoch 0, the test Accuracy is better than Train accuracy. It
continues this way until Epoch 10, then after 10th epoch Train accuracy is more than Test
accuracy where the model tries to overfit & doesn’t do well on Test data.

Model loss summary : At epoch 0, the test loss is less than Train loss. It continues this way
until Epoch 3, then Train loss is same as Test loss.

I used Grid search to get the best parameters for achieving best accuracy & are as follows :
Embedding dimension : 128,
Embedding_regularizer : None,
Num of conv_layers : 1,
Num of fc_layers : 1,
Batch_size : 256
Best accuracy : 87.26% on Validation dataset
