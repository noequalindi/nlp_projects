# Sentiment Analysis of Reviews

1. Entrenar un modelo de clasificación para el dataset propuesto (reviews de apps) utilizando BERT como encoder fijo (pesos freezados) y entrenando solamente la última parte de la red para clasificación. La elección de la arquitectura de la última parte queda a su criterio (pueden usar densas, recurrentes, convolucionales o lo que sea).
2. Encaren el problema con la reducción de 3 clases y el problema original con 5 clases. Muestren los resultados de desempeño en cada caso.
Trabajar a partir de la notebook que vimos en clase:
[Notebook Clase 7](https://github.com/FIUBA-Posgrado-Inteligencia-Artificial/procesamiento_lenguaje_natural/blob/main/clase_7/jupyter_notebooks/tensorflow/7d%20-%20bert%20sentiment%20analysis%20multicategorial.ipynb)

Datasets: 
[apps.csv](https://drive.google.com/u/0/uc?id=1S6qMioqPJjyBLpLVz4gmRTnJHnjitnuV&export=download&confirm=t)
[reviews.csv](https://drive.google.com/u/0/uc?id=1zdmewp7ayS4js4VtrJEHzAheSW-5NBZv&export=download&confirm=t)

### Requisitos
`python ^3.10`

### Colab
[model_3_classes_fine_tuning](https://colab.research.google.com/drive/1p07TFdqyEyjyshoqsSgQuSbr_y7ARg2j?usp=sharing)
[model_3_classes_no_fine_tuning](https://colab.research.google.com/drive/1e0PGS5iT7GM-ckSFCJ05hs4lcL8K_lVu?usp=sharing)
[model_5_classes_no_fine_tuning](https://colab.research.google.com/drive/1IxbN5n8TRUdF5EkSMmh7KUjn8J-LzJ3g?usp=sharing)
