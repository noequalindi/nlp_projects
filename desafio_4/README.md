# Chatbot QA with LSTM

1. Construir QA Bot basado en el ejemplo del traductor pero con un dataset QA.

Recomendaciones:
- MAX_VOCAB_SIZE = 8000
- max_length ~ 10
- Embeddings 300 Fasttext
- n_units = 128
- LSTM Dropout 0.2
- Epochs 30~50

Dataset: [data_volunteers.json](https://drive.google.com/uc?id=1awUxYwImF84MIT5-jCaYAPe2QwSgS1hN&export=download)

### Requisitos 
`python ^3.10`

### Colab 
[Chatbot QA]{https://colab.research.google.com/drive/1fQyH7ht-W690_l334LhMmsBMkTr_OMrV?usp=sharing}