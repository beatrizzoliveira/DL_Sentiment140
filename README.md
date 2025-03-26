# Deep Learning - Sentiment 140

## Sobre o Projeto
O objetivo deste projeto é resolver um problema de **Deep Learning** utilizando redes neurais em **TensorFlow/Keras**.

## Objetivo
O projeto procura:
- Definir um problema de **Deep Learning** relevante.
- Desenvolver um modelo baseado em **redes neurais**.
- Aplicar técnicas de **pré-processamento de dados**, **tuning de hiperparâmetros** e **avaliação de desempenho**.
- Apresentar conclusões sobre a utilidade e limitações do modelo.

## Estrutura do Repositório
- `dl_sentiment140.ipynb` → Código do projeto em Jupyter Notebook.
- `requirements` → Dependencies utilizadas no projeto
- `README.md` → Documento explicativo do projeto.

## Metodologia
Seguindo as diretrizes do projeto, adotamos o seguinte workflow:

**Recolha de dado**s – Uso do dataset Sentiment140 para análise de sentimentos.

**Pré-processamento** – Tokenização, remoção de stopwords e lematização.

**Modelo** – Implementação de uma rede neural LSTM bidirecional.

**Treino e Avaliação** – Divisão dos dados (Hold-out split), uso da métrica de acurácia.

**Aprimoramento do modelo** – Uso de Dropout, tuning de hiperparâmetros, regularização.

**Interpretação dos Resultados** – Análise de métricas como matriz de confusão e gráficos de perda/acurácia.

## Principais Conclusões
- O modelo LSTM bidirecional apresentou bons resultados na classificação de sentimentos.
- Dropout e Early Stopping ajudaram a evitar overfitting.
- Possíveis melhorias incluem o uso de embeddings pré-treinados para aprimorar a representação dos textos.
- O modelo pode ser aplicado a sistemas de análise de sentimentos em tempo real.

## Contribuintes
- Beatriz Oliveira (@beatrizzoliveira)

