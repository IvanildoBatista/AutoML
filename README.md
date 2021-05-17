# Sobre o repositório

Nesse repositório irá constar projetos onde foram aplicadas ferramentas e bibliotecas de automação de processos de *data science* como modelagem e visualização de dados. Abaixo segue alguns projetos desenvolvidos:

**Auto ML para modelar aluguéis (PyCaret)**: Modelagem do preço de alugueis de casas e apartamentos no Brasil. Foi utilizada a biblioteca *PyCaret* para todas as etapas do projeto (tratamento, modelagem, avaliação, salvamento e carregamento); o modelo gerado foi um *Gradient Boosting Regressor* que obteve as melhores métricas de avaliação na validação cruzada. O R-squared do modelo foi de **0.9968**.

**Auto ML para identificação de risco de câncer (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* para modelar dados de características de pacientes e suas biópsias, para identificar qual o risco de possuir ou não câncer cervical (ou do colo do útero). O modelo gerado foi um *CatBoost Classifier* com uma acurácia de **0.9419**.

**Auto ML segmentação de clientes (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* gerar *clusters* (ou grupos) de clientes de uma empresa de cartão de crédito. Apliquei três algoritmos de *machine learning* que foram o *K-Means*, o *Agglomerative* e o *Birch*; e cada uma desses algoritmos gerou 4 grupos de clientes, mas com proporções diferentes. Essas técnicas permitiu a identificação de grupos de clientes que possuem maiores balanços (dinheiro guardado para realizar compras), maiores valores de compras e maiores valores de compras a prazo.

**Auto ML detecção de anomalias (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* identificar anomalias em uma base de cartões de créditos e depois analisar se as anomalias identificadas são ou não fraudes. Foram aplicados três modelos (*Iforest*, *Histogram* e *PCA*) e dos modelos o que gerou um melhor resultado foi o *PCA*, pois 432 anomalias foram identificadas como fraudes (de um total de 492).

**Auto ML para previsão de preços de casas (TPOT)**: Aplicação da biblioteca *TPOT* para previsão de preços de casas. Nesse projeto utilizei 4 métodos de seleção de *features* (por correlação, por *Feature Importance* do modelo de árvore de regressão, por *RFE* e por *PCA*) e o modelo de melhor desempenho foi aquele cuja seleção foi via correlação. O modelo gerado foi *RandomForestRegressor(RidgeCV(input_matrix), bootstrap=True, max_features=0.55, min_samples_leaf=5, min_samples_split=14, n_estimators=100)*.

Os resultado podem ser vistos abaixo:

|Método de seleção de *features* | *R-squared*     |  Erro absoluto médio  |  Erro quadrado médio|  Raiz do erro quadrado médio |
|:----------------:|:------------------:|:------------------:|:------------------:|:------------------: |
|**Correlação** | **83.8%**| **20588.527** | **1136124027.754**|**33706.439**|
|*RFE* | 0.827| 21693.596 | 1212389885.253| 34819.39 |
|*Feature Importance* | 0.716| 29641.191 | 1989657290.949| 44605.575 |
|*PCA* | 0.211| 52247.883 |5526554661.733| 74340.801 | 

**AutoML para classificação de preços de celulares (TPOT)**: Aplicação da biblioteca de *AutoML TPOT* para classificação de preços de celulares. Com o uso dessa biblioteca foi gerado um modelo com uma acurácia de **97.4%**.

**AutoML para previsão de resistência do concreto (Auto-Sklearn)**: Utilizando a biblioteca *Auto-Sklearn* para previsão de resistência de concreto; o modelo gerado pela biblioteca gerou previsões que resultaram nas seguintes métricas de avaliação abaixo:

|Métrica | Resultado |
|:----------:|:------------------:|
|*R-squared*| 89.803 %|
|Erro médio absoluto | 3.907485038152961|
|Erro médio percentual absoluto |0.13186784887581904|
|Erro médio quadrado |27.62182916624647|
|Erro médio logarítmico quadrado|0.026504404779111895|
|Erro mediano absoluto|2.848742341995239|

**AutoML para previsão Churn de clientes (Auto-Sklearn)**: O melhor modelo foi o que utilizou a algoritmos de reamostragem Instance Hardness Threshold que obtive as melhores métricas de avaliação;

**Automatização de visualização de dados (AutoViz)**: Aplicação da biblioteca *AutoViz* para automatizar o processo de visualização de uma base de dados de carros usados. Foram gerados os gráficos *Scatterplot*, *Pairwise-plot*, Histograma, *Boxplots*, *QQplot*, *Violinplot*, *Heatmap*, *Pivot Table* e  *barplots* e, com esses gráficos, foi possíveis identificar:

1) a relação positiva entre a variável *engineSize* e o preço (*price*, variável alvo);

2) As variáveis contínuas não possuem uma distribuição normal, o que pode ser um problema na hora de passá-las para modelos de *machine learning* ou de *deep learning*, pois alguns desses modelos pressupõem normalidade nas variáveis e isso mostra que essas colunas precisam de algum tipo de tratamento (normalização ou padronização). Outra coisa que pode-se notar é a presença de muitos *outliers* na variável *price* que pode ser ruim para o treinamento de um modelo, então essa coluna pode requerer um tratamento.
