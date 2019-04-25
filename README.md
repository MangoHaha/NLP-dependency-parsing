# NLP-dependency-parsing

### Input Layer
Word features: 20 types of word features.
Part-of-speech features: 20 types of POS features.
Dependency label features: 12 types of dependency features.

### Embedding Layer
Word embedding with dimension dw. 
IfFirst Hidden Layer the training corpus has Nw unique words, the size of the embedding dictionary will be dw\*Nw

Part-of-speech embedding with dimension dt.
the size of the embedding dictionary will be dt\*Nt, if the training corpus has Nt unique POS tags

Dependency label embedding with dimension dl.
If the training corpus has Nl unique dependency labels, the size of the embedding dictionary will be dl\*Nl.

Thus the output from the embedding layer e, is the concatenation of all embedding values for the specific data instance.
  de = 20(dw + dt) + 12dl


  
### Hidden Layer 

The first hidden layer: output of the embedding layer e should be fed to the first hidden layer with a rectified linear unit (RELU) activation.

The second hidden layer: output of the first hidden layer h1 should be fed to the second hidden layer
with a rectified linear unit (RELU) activation.

### output Layer
Finally, the output of the second hidden layer h2 should be fed to the output layer with a softmax activation function.





