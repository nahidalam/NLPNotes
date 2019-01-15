# Notes on Natural Language Processing (NLP) - Log

## I plan to learn and do hands on code on
1. Word Embedding
  - learn to use word2vec and/or BERT in Sentiment Analysis
2. RNN and its variants like LSTM, bi-LSTM
  - Implement LSTM in some problem
3. Language models - ELMo, ULMFit, BERT  and code them up

## Day 1 : Jan 2, 2019

**Today's Progress** : n-gram model, Bag-of-Word(BoW), Tf-Idf

## Day 2 : Jan 3, 2019

**Today's Progress** :
- Word Embedding https://github.com/nahidalam/NLPNotes/blob/master/2_WordEmbedding.md
- Parse Tree https://github.com/nahidalam/NLPNotes/blob/master/2_ParseTree.md

## Day 3: Jan 4, 2019

**Today's Progress** : POS Tagging, Build your own POS tagger

## Day 4: Jan 5, 2019
**Today's Progress** :
- Build your own POS tagger (continued) https://github.com/nahidalam/NLP_Study_Group/tree/master/7_Weeks_NLP_Projects/Week4_POSTagger

## Day 5: Jan 6, 2019
**Today's Progress** : Worked on a cuisine prediction service. Built the model and wrote a web service to display results based on the predictive model https://github.com/nahidalam/cuisine_prediction_service

## Day 6: Jan 7, 2019
**Today's Progress** :

- Revisited RNN, LSTM (and variants like Peephole Connection), GRU
- LSTM vs. GRU
- Beam Search https://www.youtube.com/watch?v=RLWuzLLSIgw
- BLEU Score (essentially a MT metrics - how good a generated sentence is)
- Attention paper explanation https://mlexplained.com/2017/12/29/attention-is-all-you-need-explained/

## Day 7: Jan 8, 2019
**Today's Progress** :
- Overview on BERT. Lot to digest but at least got an idea about the transfer learning literature in NLP https://mlexplained.com/2019/01/07/paper-dissected-bert-pre-training-of-deep-bidirectional-transformers-for-language-understanding-explained/

## Day 8: Jan 9, 2019
**Today's Progress** :
- Naive Bayes and its usage in Sentiment analysis. Why Naive Bayes helps in reducing runtime complexity (because of its assumption that features are independent from each other) https://www.datacamp.com/community/tutorials/simplifying-sentiment-analysis-python
- Sentiment analysis using Word Embedding (word2vec), LSTM, Keras  https://ahmedbesbes.com/sentiment-analysis-on-twitter-using-word2vec-and-keras.html
https://www.liip.ch/en/blog/sentiment-detection-with-keras-word-embeddings-and-lstm-deep-learning-networks
- **TODO** Sentiment analysis using BERT embedding https://github.com/brightmart/sentiment_analysis_fine_grain
https://gluon-nlp.mxnet.io/examples/sentence_embedding/bert.html

## Day 9: Jan 10, 2019
**Today's Progress** :
- Finished this Datacamp course on Deep Learning with Python and Keras. https://campus.datacamp.com/courses/deep-learning-in-python
I did some projects with Keras before, outside of my job sometimes in mid 2017. So it was a good refresher.

## Day 10: Jan 11, 2019
**Today's Progress** :
- Setup Domino Data Lab for some project submission in SpringBoard
- Generative vs. Discriminative Models
https://stackoverflow.com/questions/879432/what-is-the-difference-between-a-generative-and-a-discriminative-algorithm
https://medium.com/@mlengineer/generative-and-discriminative-models-af5637a66a3

## Day 11: Jan 12, 2019
**Today's Progress** :
- Trying to understand how LSTM is used in the dialog management in Rasa https://forum.rasa.com/t/understanding-the-usage-of-lstm-in-keras-policy/4278
- Implement LSTM in Keras for sentiment analysis https://towardsdatascience.com/understanding-lstm-and-its-quick-implementation-in-keras-for-sentiment-analysis-af410fd85b47

## Day 12: Jan 13, 2019
**Today's Progress** :
- Reviewed SQL JOINS and some Data Wrangling techniques (not really NLP)
- Advanced Deep Learning with Keras. Interesting advanced techniques when you have multiple inputs in the input layer. Not going deep into the course but will use some of it in the capstone project https://www.datacamp.com/courses/advanced-deep-learning-with-keras-in-python

## Day 13: Jan 14, 2019
**Today's Progress** :
- Learned about Explainable ML https://christophm.github.io/interpretable-ml-book
Example explainable models are - Linear Regression, DT, Logistic Regression etc. Interesting that Neural Network models are not explainable. But I guess we can use the model agnostic characteristics (such as feature importance, feature relations etc.) while using Neural Networks.
- Explainable Neural Network https://distill.pub/2018/building-blocks/
- Finalized the capstone project proposal
