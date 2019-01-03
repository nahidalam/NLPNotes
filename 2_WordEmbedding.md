# Word Embedding
- Dense representation
- Distributed representation/vector - meaning each element represents a property, and they are shared between the words. For example: suppose we are representing animals based on 3
properties - furry, dangerous, mammals. Now if we want to categorize animals
(e.g. bears, cats, dogs, frogs etc.) based on those 3 properties, each property will
have some number in the range of 0-1 depending on how representative those animals
are wrt. those properties. For example - bear can be furry = 0.9, dangerous = 0.85,
mammals = 1.0 etc.
- This distributed representation essentially groups similar things closer.
Mathematically, the cosine of the angle between such vectors should be close to
1, i.e. angle close to 0.
- So we can infer some information about words based on their vectors. We don't
even need any label. That's AMAZING!
- Shallow Neural Network (only one hidden layer) - more on this later.




### How to Create these word vectors:
One way is to use count based vectors - one hot so sparse.

Other way is - **Neural Word Embedding** which is what this topic is about

### So how do we create these word embeddings?
Word2Vec is a way to create these word embeddings.

To summarize the above based on the Kaggle article -

Word2vec is a neural network implementation that learns distributed representations for words.
Word2Vec does not need labels in order to create meaningful representations. This is useful, since most data in the real world is unlabeled. If the network is given enough training data (tens of billions of words), it produces word vectors with intriguing characteristics. Words with similar meanings appear in clusters, and clusters are spaced such that some word relationships, such as analogies, can be reproduced using vector math. The famous example is that, with highly trained word vectors, "king - man + woman = queen."


## Types of Word Embedding
There are 2 common Word Embedding models - Word2Vec and GloVe

Then again, Word2Vec is 2 types
- Skip Gram and
- Continuous Bag Of Words (CBOW)

**CBOW Model**:
- Predict the current word, based on the surrounding words. In most cases, this
is just predicting 1 word based on the 1 closest word.

Example sentence: Have a great day

Suppose out input is 'great' and we want to predict the next word 'day'. we use the one hot encoding of the input word and measure the output error compared to one hot encoding of the target word (day). In the process of predicting the target word, we learn the vector representation of the target word [4].

![CBOW based on one context word](./cbow-one-word-contect.png)

**Skip Gram Model**:
- Predict the surrounding words, based on the current word.




### When to use pre-trained Word Embedding or not?

### What are the issues with Word2Vec?

### Word2Vec vs GloVe

### How to make these models computationally more efficient

**Reference**:
1. Google code https://code.google.com/archive/p/word2vec/
2. Original NIPS 2013 presentation https://docs.google.com/file/d/0B7XkCwpI5KDYRWRnd1RzWXQ2TWc/edit
3. http://www.marekrei.com/pub/Constructing_and_Evaluating_Word_Embeddings.pdf
4. https://towardsdatascience.com/introduction-to-word-embedding-and-word2vec-652d0c2060fa
5. https://www.kaggle.com/c/word2vec-nlp-tutorial#part-2-word-vectors
