# Esteira de aprendizado de máquina: Classificação binária de músicas como virais ou não-virais
Este notebook implementa uma esteira de aprendizado de máquina para um problema de classificação binária, a fim de prever se uma música será viral ou não. O dataset utilizado é o "What Makes a Song Viral?", disponível em: https://www.kaggle.com/datasets/vedauv/what-makes-a-song-go-viral-10000-tracks/data?select=viral_songs.csv. 

As etapas são: análise de estatísticas do dataset, tratamento de dados (remoção de linhas e colunas), criação de subconjuntos de treinamento, validação e teste, treinamento com o algoritmo XGBoost no Amazon SageMaker, inferência em lote, avaliação por meio de matriz de confusão e outras métricas e a inferência em tempo real.

Como executar: abra o notebook em um ambiente do Amazon SageMaker, coloque o arquivo viral_songs.csv na mesma pasta do notebook e execute as células em ordem, de cima para baixo.
