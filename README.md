# NLP Projects

![image](https://github.com/user-attachments/assets/3b0d82e4-f63c-4e88-bc61-773b55d4fb77)

## Project 1 - Vectorization & Naïve Bayes Classificantion 
Se realizó una vectorización de documentos como también la realización de entrenamientos de distintos modelos de Bayes. La consigna principal era realizar un primer acercamiento a lo que son los embeddings a través de la transposición de la matríz documento-término.
Dataset: `fetch_20newsgroups`

## Project 2 - Custom Embeddings & Gensim - Word2Vec
Se utilizaron embeddings con word2Vec, con diferentes técnicas como Skip-Gram y CBOW. Se utilizó un corpus de texto literario: [Orgullo y Prejuicio - Jane Austen](https://www.textos.info/jane-austen/orgullo-y-prejuicio)
y se emplearon técnicas de reducción de dimensionalidad provistas en clase como PCA y T-SNE, para tipos de modelos de lenguaje grande (LLM) como el que se utilizó.

## Project 3 - Tokenization by word & char
Se probaron distintas estrategias para conseguir el mejor modelo de lenguaje. Estrategias utilizadas: Greedy y Beam, con diferentes unidades recurrentes (SimpleRNN, LSTM, GRU).
El corpus de texto utilizado: [Orgullo y Prejuicio - Jane Austen](https://www.textos.info/jane-austen/orgullo-y-prejuicio)

## Project 4 - QA Chatbot LSTM & GloVe embeddings
Se utilizó una arquitectura encoder-decoder con unidades recurrentes LSTM. 
Dataset: `data_volunteers.json` disponible en la carpeta.

![alt text](img/image-3.png)
![alt text](img/image-4.png)

## Project 5 - Sentiment Analysis using Transfer Learning & BERT
Se utilizó el modelo BERT base, y se realizó transfer learning. 
Se realizaron distintas estrategias como:
- No descongelamiento de capas para modelos con 3 y 5 clases de salida.
- Fine Tuning descongelando todas las capas, con 3 clases de salida.
- En el caso de las 3 clases, se aplico un balanceo de la variable `score` como `sentiment`, las cuales tendrán de salida `[negative, neutral, positive]`

El modelo elegido para este ejemplo es al que se le realizo fine tuning ya que es el que mejor accuracy y precisión tuvo: 

![alt text](img/image-1.png)
![alt text](img/image.png)
![alt text](img/image-2.png)