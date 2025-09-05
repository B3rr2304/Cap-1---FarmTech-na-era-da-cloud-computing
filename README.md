Previsão de Rendimento de Safra com Machine Learning (Etapa 1)
Objetivo
Desenvolver um modelo de Machine Learning para prever o rendimento de safras agrícolas, permitindo que a empresa FarmTech Solutions otimize seu planejamento e tomada de decisão com base em dados climáticos.

Variáveis do Dataset Utilizadas
Cultura: Identificação do tipo de plantação (ex: Trigo, Arroz).

Precipitação (mm dia 1): Volume de chuva diário.

Umidade Específica e Relativa: Medidas da quantidade de vapor de água no ar.

Temperatura (ºC): Temperatura do ar a 2 metros de altura.

Rendimento: A variável alvo, representando a produção em toneladas por hectare.

Funcionamento
Os dados do arquivo crop_yield.csv são carregados em um ambiente Python para análise.

É realizada uma Análise Exploratória dos Dados (EDA) para entender as variáveis, suas distribuições e correlações.

Os dados são segmentados em diferentes perfis de produção através de clusterização (K-Means).

Outliers (cenários discrepantes) são identificados com o algoritmo DBSCAN e removidos para garantir a robustez do modelo.

Cinco diferentes modelos de Machine Learning são treinados, com os dados devidamente escalonados, para prever o Rendimento.

Os modelos são avaliados com métricas como R², MAE e RMSE, e o de melhor desempenho é selecionado como a solução final.

Principais Achados da Análise
Foi observada uma clara correlação positiva entre as variáveis de umidade e o rendimento final da safra.

Os modelos de ensemble (Random Forest e Gradient Boosting) apresentaram desempenho superior, indicando que as relações entre o clima e o rendimento são complexas e não-lineares.

O pré-processamento de escalonamento dos dados mostrou-se um passo fundamental, melhorando drasticamente o desempenho de algoritmos como k-NN e SVR.

Principais Visualizações
Dentro do Notebook Jupyter, você encontrará os seguintes gráficos que resumem o projeto:

Mapa de Calor de Correlações: Quantifica a relação linear entre todas as variáveis.

Gráfico de Clusters: Visualiza os diferentes perfis de produção agrícola encontrados nos dados.

Gráfico Comparativo dos Modelos: Apresenta o desempenho (R², MAE, RMSE) dos cinco modelos, facilitando a identificação do modelo campeão.

Análise de Custos em Nuvem (AWS) (etapa 2)
Esta seção detalha a análise comparativa de custos para hospedar a solução de Machine Learning na nuvem AWS, comparando as regiões de São Paulo (Brasil) e Virgínia do Norte (EUA).

Análise Comparativa de Custos
O objetivo foi estimar o custo mensal para um servidor com a configuração de 2 CPUs, 1 GiB de memória, até 5 Gigabit de rede e 50 GB de armazenamento, utilizando o modelo de preço On-Demand (Sob Demanda). A simulação foi realizada na Calculadora de Preços da AWS em 04 de setembro de 2025.

Organização do Repositório
Bernardo_Zandoná_Rupolo_565182_pbl_fase4.ipynb: Notebook Jupyter contendo todo o código e a análise detalhada, desde a exploração dos dados até a conclusão final.

crop_yield.csv: O conjunto de dados original utilizado para o treinamento e análise.

README.md: Este arquivo, com a documentação resumida do projeto.

Links para Avaliação
https://colab.research.google.com/drive/1BzMj1E4WHzvJ3FzNyqqDZfmGdurAuaTa#scrollTo=7LbVrDSJS6Kd
https://youtu.be/QJj91ve45Es
https://youtu.be/_bncHSfU6yM
