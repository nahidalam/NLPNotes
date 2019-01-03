# Word Embedding
- Dense representation
- Distributed representation/vector - meaning each element represents a property, and they are shared between the words. For example: suppose we are representing animals based on 3
properties - furry, dangerous, mammals. Now if we want to categorize animals
(e.g. bears, cats, dogs, frogs etc.) based on those 3 properties, each property will
have some number in the range of 0-1 depending on how representative those animals
are wrt. those properties. For example - bear can be furry = 0.9, dangerous = 0.85,
mammals = 1.0 etc.
- This distributed representation essentially groups similar things closer
- So we can infer some information about words based on their vectors. We don't
even need any label. That's AMAZING!


### How to Create these word vectors:
One way is to use count based vectors - one hot so sparse.

Other way is - **Neural Word Embedding** which is what this topic is about

### So how do we create these word embeddings?


## Types of Word Embedding


### When to use pre-trained Word Embedding or not?

### What are the issues with Word2Vec?

### Word2Vec vs GloVe

**Reference**:
- http://www.marekrei.com/pub/Constructing_and_Evaluating_Word_Embeddings.pdf
