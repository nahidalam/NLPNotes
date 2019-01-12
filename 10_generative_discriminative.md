## Generative vs. Discriminative Models

Let's say you have input data `x` and you want to classify the data into labels `y`.

A **generative model** learns the joint probability distribution `p(x,y)`
- A Generative Model ‌explicitly models the actual distribution of each class. E.g. GAN, Naïve Bayes, Bayesian networks, Markov random fields, ‌Hidden Markov Models (HMM)

A **discriminative model** learns the conditional probability distribution `p(y|x)`
- A Discriminative model ‌models the decision boundary between the classes. E.g. SVM, DT, CRF, Logistic Regression, traditional Neural Nets


### Reference:
1. https://stackoverflow.com/questions/879432/what-is-the-difference-between-a-generative-and-a-discriminative-algorithm
2. http://cs229.stanford.edu/syllabus.html
3. http://ai.stanford.edu/~ang/papers/nips01-discriminativegenerative.pdf
