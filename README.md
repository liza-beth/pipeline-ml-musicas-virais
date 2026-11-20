# Esteira de aprendizado de máquina: músicas virais

Projeto da disciplina Inteligência Artificial. O notebook implementa uma esteira completa de classificação binária que prevê se uma música será **viral** ou **não viral**.

- **Dataset:** [What Makes a Song Viral? (Kaggle)](https://www.kaggle.com/datasets/vedauv/what-makes-a-song-go-viral-10000-tracks/data?select=viral_songs.csv), arquivo `viral_songs.csv`, 10 mil registros.
- **Algoritmo:** XGBoost (SageMaker)

### Passos do notebook
1. Importar dataset
2. Estatísticas descritivas e gráficos de densidade e de caixa.
3. Tratamento das linhas (valores ausentes, duplicados e inválidos) e das colunas (remoção de colunas de identificação e de `streams`, que entrega a resposta; one-hot encoding de `genre`).
4. Matriz de correlação.
5. Divisão em subconjuntos de treinamento (80%), validação (10%) e teste (10%).
6. Treinamento do XGBoost no SageMaker.
7. Inferência em lote.
8. Avaliação: matriz de confusão, acurácia, sensibilidade, especificidade, precisão.
9. Implantação do modelo em um endpoint e uma predição em tempo real.

## Como executar

1. Baixe o dataset no [Kaggle](https://www.kaggle.com/datasets/vedauv/what-makes-a-song-go-viral-10000-tracks/data?select=viral_songs.csv) e salve o arquivo `viral_songs.csv`.
2. Em um ambiente AWS, crie um notebook no SageMaker AI. Adicione o arquivo .ipynb e o dataset.
3. Execute todas as células em oredem.
