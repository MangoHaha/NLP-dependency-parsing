# NLP-dependency-parsing

Input Layer
Word features: 20 types of word features.
Part-of-speech features: 20 types of POS features.
Dependency label features: 12 types of dependency features.

Embedding Layer
Word embedding with dimension dw. 
If the training corpus has Nw unique words, the size of the embedding dictionary will be dw\*Nw

Part-of-speech embedding with dimension dt.
the size of the embedding dictionary will be dt\*Nt, if the training corpus has Nt unique POS tags

Dependency label embedding with dimension dl.
If the training corpus has Nl unique dependency labels, the size of the embedding dictionary will be dl\*Nl.

Thus the output from the embedding layer e, is the concatenation of all embedding values for the specific data instance.
  de = 20(dw + dt) + 12dl
  
  




