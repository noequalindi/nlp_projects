# NLP Projects

![image](https://github.com/user-attachments/assets/3b0d82e4-f63c-4e88-bc61-773b55d4fb77)

## Project 1 - Vectorization & Naïve Bayes Classificantion 
Propósito: La consigna principal era realizar un primer acercamiento a lo que son los embeddings a través de la transposición de la matríz documento-término.
Se realizó la vectorización de documentos y los entrenamientos correspondientes de distintos modelos de Bayes. 

### Dataset: 
`fetch_20newsgroups` de `sklearn`

### Colab
[Vectorization - Naive Bayes](https://colab.research.google.com/drive/1G2OT0OlJ7hcDNuO1HTaxpVejN6V0NPsB?usp=sharing)

## Project 2 - Custom Embeddings & Gensim - Word2Vec
Objetivo: Mejorar la representación semántica de las palabras en el corpus y analizar la estructura de los embeddings en un espacio reducido.
Se utilizaron embeddings con word2Vec, con diferentes técnicas como Skip-Gram y CBOW. Se utilizó un corpus de texto literario: [Orgullo y Prejuicio - Jane Austen](https://www.textos.info/jane-austen/orgullo-y-prejuicio)
y se emplearon técnicas de reducción de dimensionalidad provistas en clase como PCA y T-SNE, para tipos de modelos de lenguaje grande (LLM) como el que se utilizó.

### Colab
[Custom Embeddings con Gensim](https://colab.research.google.com/drive/16zILcrn9sXVkJqFuoVHLTsjq8GQPsdYB?usp=sharing)

## Project 3 - Tokenization by word & char
Propósito: El objetivo era predecir la próxima palabra o carácter en una secuencia de texto.
Se probaron distintas estrategias para conseguir el mejor modelo de lenguaje. Estrategias utilizadas: Greedy y Beam search, con diferentes tipos de redes recurrentes (SimpleRNN, LSTM y GRU).

El corpus de texto utilizado: [Orgullo y Prejuicio - Jane Austen](https://www.textos.info/jane-austen/orgullo-y-prejuicio)

### Colab links
1. [Tokenización por palabra](https://colab.research.google.com/drive/1LkWok653p_4QlKI_Vp4QyFv6_X_8fDnz?usp=sharing)
2. [Tokenización por caracter](https://colab.research.google.com/drive/1v4nmvaJFaCdGGgVL-VmF37ALu9KC36-F?usp=sharing)

## Project 4 - QA Chatbot LSTM & GloVe embeddings
Propósito: Desarrollar un chatbot de preguntas y respuestas (QA) que pueda gestionar y responder consultas efectivamente.
Se utilizó una arquitectura encoder-decoder con unidades recurrentes LSTM. Se emplearon embeddings GloVe para representar los datos textuales.
Dataset: `data_volunteers.json` disponible en la carpeta.

![alt text](img/image-3.png)
![alt text](img/image-4.png)

Dataset: [data_volunteers.json](https://drive.google.com/uc?id=1awUxYwImF84MIT5-jCaYAPe2QwSgS1hN&export=download)

### Requisitos 
`python ^3.10`

### Colab 
[Chatbot QA](https://colab.research.google.com/drive/1fQyH7ht-W690_l334LhMmsBMkTr_OMrV?usp=sharing)

## Project 5 - Sentiment Analysis using Transfer Learning & BERT
Propósito: Hacer un análisis de sentimiento de las reseñas de distintas aplicaciones y clasificarlas.   
Se utilizó el modelo BERT base, y se realizó transfer learning. 
Se realizaron distintas estrategias como:
- Sin fine tuning para modelos con 3 y 5 clases de salida.
- Fine Tuning completo, con 3 clases de salida.
- En el caso de las 3 clases, tanto con y sin fine tuning, se aplicó un balanceo de la variable `score` a `sentiment`, con el objetivo de convertir las etiquetas originales en tres categorías más significativas para la clasificación de sentimientos: `[negative, neutral, positive]`

### Datasets: 
1. [apps.csv](https://drive.google.com/u/0/uc?id=1S6qMioqPJjyBLpLVz4gmRTnJHnjitnuV&export=download&confirm=t)
2. [reviews.csv](https://drive.google.com/u/0/uc?id=1zdmewp7ayS4js4VtrJEHzAheSW-5NBZv&export=download&confirm=t)

### Requisitos:
`python ^3.10`

### Colab links
1. [model_3_classes_fine_tuning](https://colab.research.google.com/drive/1p07TFdqyEyjyshoqsSgQuSbr_y7ARg2j?usp=sharing)
2. [model_3_classes_no_fine_tuning](https://colab.research.google.com/drive/1e0PGS5iT7GM-ckSFCJ05hs4lcL8K_lVu?usp=sharing)
3. [model_5_classes_no_fine_tuning](https://colab.research.google.com/drive/1IxbN5n8TRUdF5EkSMmh7KUjn8J-LzJ3g?usp=sharing)

### Disponibilización del modelo entrenado | arquitectura + pesos entrenados
- [BERT model - weights](https://drive.google.com/drive/folders/1aOPDlwsYyvBEx7-pZZ66-ctb-50mgMzJ)

El modelo elegido para este ejemplo es al que se le realizó fine tuning, con el mejor rendimiento. 

![alt text](img/image-1.png)
![alt text](img/image.png)
![alt text](img/image-2.png)
