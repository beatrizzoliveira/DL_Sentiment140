# Deep Learning - Sentiment 140

## Sobre o Projeto
Este projeto implementa um modelo de deep learning para análise de sentimentos em tweets usando o dataset **Sentiment140**. O modelo foi desenvolvido utilizando **redes neurais LSTM**, que são eficazes para processar sequências de texto.

## Objetivo
Criar um modelo capaz de classificar tweets como positivos ou negativos, auxiliando na análise automática de opiniões expressas nas redes sociais.

## Estrutura do Repositório
- `DL_sentiment140.ipynb` → Código do projeto em Jupyter Notebook.
- `requirements.txt` → Dependências utilizadas no projeto.
- `README.md` → Documento explicativo do projeto.

## Pipeline do Projeto
1. **Recolha e Pré-processamento de Dados**
   - Remoção de caracteres especiais e links.
   - Tokenização dos textos.
   - Conversão de palavras para vetores (word embeddings).
   - Remoção de stopwords e lematização.

2. **Construção do Modelo**
   - Uso de uma camada de embedding para representar palavras.
   - Implementação de uma rede neural LSTM bidirecional.
   - Camada densa final com ativação sigmoide para classificação binária.
   - Uso de Dropout para evitar overfitting.

3. **Treinamento e Avaliação**
   - Utilização de função de perda `binary_crossentropy`.
   - Otimização com `Adam`.
   - Divisão dos dados (Hold-out split) para avaliação.
   - Avaliação da acurácia com `model.evaluate`.
   - Análise de métricas como matriz de confusão e gráficos de perda/acurácia.

## Decisões Técnicas
- **Por que LSTM bidirecional?**
  - Redes LSTM são adequadas para processar texto, pois mantêm informações ao longo da sequência, e a versão bidirecional permite capturar relações no contexto anterior e posterior.
- **Por que embeddings?**
  - Embeddings transformam palavras em vetores densos que preservam relações semânticas.
- **Aprimoramento do modelo**
  - Uso de Dropout, tuning de hiperparâmetros e regularização.

## Resultados
- A acurácia final pode ser obtida ao rodar `model.evaluate` no conjunto de testes.
- O modelo pode ser ajustado com mais dados ou técnicas como fine-tuning de embeddings pré-treinados.

## Principais Conclusões
- O modelo LSTM bidirecional apresentou bons resultados na classificação de sentimentos.
- Dropout e Early Stopping ajudaram a evitar overfitting.
- Possíveis melhorias incluem o uso de embeddings pré-treinados para aprimorar a representação dos textos.
- O modelo pode ser aplicado a sistemas de análise de sentimentos em tempo real.

## Conclusão
O modelo LSTM implementado apresenta um bom desempenho na classificação de sentimentos em tweets e pode ser aprimorado com mais dados e ajustes nos hiperparâmetros. Ele pode ser aplicado em diversas áreas, como monitoramento de redes sociais e análise de feedbacks.

## Como Executar
1. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
2. Execute o notebook:
   ```bash
   jupyter notebook DL_Sentiment140.ipynb
   ```
3. Treine e avalie o modelo.

## Contribuição
Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias.

## Licença
Este projeto é distribuído sob a licença MIT.

