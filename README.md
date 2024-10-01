Descrição do Projeto:
Este projeto é uma aplicação de classificação de notícias falsas e verdadeiras utilizando técnicas de processamento de linguagem natural (NLP) e regressão logística. O modelo é treinado para distinguir entre notícias reais e falsas com base no conteúdo textual das reportagens. O objetivo é construir um classificador eficiente para detectar desinformação em textos de notícias.

Funcionalidades:
Carga de Dados: O projeto carrega dois arquivos CSV - um contendo notícias falsas (Fake.csv) e outro com notícias reais (True.csv).

Preprocessamento dos Dados: O código combina as duas bases de dados, rotulando as notícias falsas com o valor 0 e as notícias reais com 1. Também remove colunas irrelevantes como 'date' e 'title', reorganizando o dataset de forma aleatória.

Vetorização TF-IDF: O conteúdo das notícias é transformado em uma representação numérica usando o TfidfVectorizer, que converte o texto bruto em vetores, facilitando o uso de algoritmos de machine learning.

Divisão dos Dados: O dataset é dividido em dados de treino e teste utilizando a função train_test_split com 20% dos dados reservados para testes.

Treinamento e Predição: O modelo de regressão logística é utilizado para treinar os dados de texto vetorizados e prever se uma notícia é falsa ou real.

Avaliação do Modelo: São calculadas métricas de desempenho como a acurácia, além de gerar a matriz de confusão para visualização dos resultados e o relatório de classificação com precisão, recall e F1-score.


Tecnologias Utilizadas:

Pandas: Para manipulação e análise dos dados.

NumPy: Para cálculos matemáticos.

Matplotlib e Seaborn: Para visualização de dados e gráficos, incluindo a matriz de confusão.

Scikit-learn: Para vetorização de texto (TF-IDF), modelagem de machine learning (Regressão Logística) e métricas de avaliação.

Google Colab: Ambiente de execução do código com suporte a upload de arquivos.


Resultados:
Acurácia: O modelo alcança uma boa taxa de acerto ao classificar as notícias como reais ou falsas.
Matriz de Confusão: Um gráfico é gerado para facilitar a visualização dos erros e acertos do modelo.
Relatório de Classificação: Exibe as métricas de precisão, recall e F1-score para cada classe (Fake e Real).

Observações sobre o Código:
O código faz uso de vetorização TF-IDF para transformar o texto das notícias em dados numéricos que podem ser processados pelo modelo de machine learning.
A regressão logística foi escolhida por sua simplicidade e eficácia em problemas de classificação binária.
O projeto permite a visualização gráfica dos resultados usando uma matriz de confusão e também apresenta um relatório detalhado sobre a performance do modelo.

