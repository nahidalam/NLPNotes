# Notes on Natural Language Processing (NLP)

## Day 1 : Jan 2 , 2019

### n-gram Model

Reference https://sookocheff.com/post/nlp/n-gram-modeling/

#### What is the difference between n-gram model and Machine Learning based NLP models?

n-gram models are probabilistic models


### Bag of Word (BoW)

Reference: https://www.kaggle.com/c/word2vec-nlp-tutorial#part-1-for-beginners-bag-of-words

The Bag of Words model learns a vocabulary from all of the documents, then models each document by counting the number of times each word appears.

#### What do we mean when we say 'our model is using BoW featurizer'?

Consider the following two sentences:

Sentence 1: "The cat sat on the hat"

Sentence 2: "The dog ate the cat and the hat"

From these two sentences, our vocabulary is as follows:

{ the, cat, sat, on, hat, dog, ate, and }

To get our bags of words, we count the number of times each word occurs in each sentence. In Sentence 1, "the" appears twice, and "cat", "sat", "on", and "hat" each appear once, so the feature vector for Sentence 1 is:

{ the, cat, sat, on, hat, dog, ate, and }

Sentence 1: { 2, 1, 1, 1, 1, 0, 0, 0 }

Similarly, the features for Sentence 2 are: { 3, 1, 0, 0, 1, 1, 1, 1}
