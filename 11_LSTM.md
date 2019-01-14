## LSTM
The web is full of LSTM explanations such as [1], [2] and [3]. I am more interested in understanding how it is applied to real problems.

For example - in **Dialog Management**. While developing chatbots - I have used Rasa (www.rasa.com). Rasa has 2 components - `Rasa NLU` and `Rasa Core`. The `Rasa Core` is responsible for Dialog Management so it will be interesting to see how they are using LSTM. I don't fully understand it yet so have asked this questions at Rasa forum ( https://forum.rasa.com/t/understanding-the-usage-of-lstm-in-keras-policy/4278).

Fundamentally, the dialog management of a chatbot is a sequence modeling task. What reply should come after what question - that is essentially similar to sequence modeling task. Think of the Beam Search example in NMT or any other Language Modeling task. Dialog Management in its core is a similar sequence modeling problem. So LSTM is used. 

Another usage is **Sentiment Analysis**. The tutorial at [4] is a short of sweet example of using LSTM for sentiment analysis. It has used Keras library for  doing that

```
embed_dim = 128
lstm_out = 200
batch_size = 32

model = Sequential()
model.add(Embedding(2500, embed_dim,input_length = X.shape[1], dropout = 0.2))
model.add(LSTM(lstm_out, dropout_U = 0.2, dropout_W = 0.2))
model.add(Dense(2,activation='softmax'))
model.compile(loss = 'categorical_crossentropy', optimizer='adam',metrics = ['accuracy'])
print(model.summary())

Y = pd.get_dummies(data['sentiment']).values
X_train, X_valid, Y_train, Y_valid = train_test_split(X,Y, test_size = 0.20, random_state = 36)

#Here we train the Network.

model.fit(X_train, Y_train, batch_size =batch_size, nb_epoch = 1,  verbose = 5)

```  

### Reference:
1. http://colah.github.io/posts/2015-08-Understanding-LSTMs/
2. https://skymind.ai/wiki/lstm
3. http://blog.echen.me/2017/05/30/exploring-lstms/
4. https://towardsdatascience.com/understanding-lstm-and-its-quick-implementation-in-keras-for-sentiment-analysis-af410fd85b47
