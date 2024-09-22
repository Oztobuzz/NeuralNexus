Theory of composition in language: smaller part -> bigger part 
E.g: words -> phrases -> sentence 

Constituency parsing: focus on breaking sentence into nested constituencies or phrases. It represents the sentence structure as a hierarchical tree.
<> 
Dependency parsing: focus on word-word relationship. Focus on showing dependency between words in sentence 


To perform Constituency parsing: -> Use recursive net (tree-like net )
<> RNN: RNN model the sequence from left to right. Cannot perform and grouping phrases recursively -> Cannot build a tree like recursive, tree net 

There are 4 big architecture for tree recursive net. Each has improvement comparing to the previous.
=> Need to have attentions for recursive net to learn something useful. (relation between words and words)
Example : Code translation from one PL -> PL 
![[Pasted image 20240826182453.png]]

Why tree recursive net is not so popular?
1. When using big enough hidden state on sequence model (RNN, LSTM, ...) has gained a considerably good result. Tree recursive net has not been proven to be better. 
2. Computational complexity: Cannot compute parallel like other architectures. Cannot optimize for GPUs 


Comparison for other model in NLP:
1. Window model (3-gram, ...): perform good on classification task. 
2. Bag of word: work rather good on classification task. Does not consider order.
3. Convnet: perform good on classification task. Especially those depend much on local information 
4. RNN: good for generating task. Not so good at classification task like convnet as it may lose useful information at the last hidden state. 
5. .....