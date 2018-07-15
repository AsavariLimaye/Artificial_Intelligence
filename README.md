# Digit Recognition using Keras

### Data

MNIST Database (using keras.datasets.mnist)


### Modules used
1. keras
2. numpy
3. matplotlib

### MNIST.ipynb
Train and test accuracy and loss vs epoch is plotted and saved as a png file.
All the models trained were moved to the folder "Models", and can be loaded and evaluated by providing the name.

### Results of Training Different Models

|Epochs|Batch Size|Optimizer|Layers| Error Function	|Train Accuracy(%)	|Test Accuracy (%)|
|---|---|---|---|---|---|---|
|30 | 10 |  sgd |sigmoid:30 sigmoid:10 | mean squared error|	91.2	|90.8|
|30 | 10 |  sgd |sigmoid:30 softmax:10 | crossentropy	|87.2	|87.5|
|00 | 10 |  sgd | sigmoid:30  softmax:10 |  crossentropy|	92.5	|92.6|
|30 | 100 |  sgd |sigmoid:30  softmax:10 |  crossentropy|	93.1	|92.7|
|200 | 100 |  sgd | sigmoid:30  softmax:10 |  crossentropy	|95.37	|94.22|
|200 | 100 |  sgd momentum 0.1 |    sigmoid:30  softmax:10 |  crossentropy|	95.2	|94.11|
|200 | 100 |  sgd momentum 0.1 |    sigmoid:100   sigmoid:80  softmax:10 |  crossentropy	|98.7	|96.4|
|200 | 100 |  sgd momentum 0.1 |   tanh100  tanh80  tanh40  softmax:10 |  crossentropy	|96	|95|
|50 | 100 |  sgd momentum 0.1 |    sigmoid:800   sigmoid:100  softmax:10 |  crossentropy	|98.4	|95.6|
|50 | 50 |  sgd momentum 0.1 |    sigmoid:784   sigmoid:80  softmax:10 |  crossentropy	|99.03	|97.06|
|100 | 50 |  sgd momentum 0.1 |    sigmoid:500   sigmoid:100   sigmoid:100  softmax:10 |  crossentropy	|99.07	|97.19|
|100 | 50 |  sgd momentum 0.1 |    sigmoid:784   sigmoid:80  softmax:10 |  crossentropy	|99.4	|97.22|
|100 | 50 | sgd momentum 0.1 |sigmoid:784 sigmoid:100 softmax:10 | crossentropy | 99.41 | 97.23|


### Best Results

|Epochs|Batch Size|Optimizer|Layers| Error Function	|Train Accuracy(%)	|Test Accuracy (%)|
|---|---|---|---|---|---|---|
|100 | 50 | sgd momentum 0.1 |sigmoid:784 sigmoid:100 softmax:10 | crossentropy | 99.41 | 97.23|




