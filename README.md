# Sobre o repositório

Nesse repositório irá constar projetos onde foram aplicadas ferramentas e bibliotecas de automação de processos de *data science* como modelagem e visualização de dados. Abaixo segue alguns projetos desenvolvidos:

**Auto ML para modelar aluguéis (PyCaret)**: Modelagem do preço de alugueis de casas e apartamentos no Brasil. Foi utilizada a biblioteca *PyCaret* para todas as etapas do projeto (tratamento, modelagem, avaliação, salvamento e carregamento); o modelo gerado foi um *Gradient Boosting Regressor* que obteve as melhores métricas de avaliação na validação cruzada. O R-squared do modelo foi de **0.9968**.

**Auto ML para identificação de risco de câncer (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* para modelar dados de características de pacientes e suas biópsias, para identificar qual o risco de possuir ou não câncer cervical (ou do colo do útero). O modelo gerado foi um *CatBoost Classifier* com uma acurácia de **0.9419**.

**Auto ML segmentação de clientes (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* gerar *clusters* (ou grupos) de clientes de uma empresa de cartão de crédito. Apliquei três algoritmos de *machine learning* que foram o *K-Means*, o *Agglomerative* e o *Birch*; e cada uma desses algoritmos gerou 4 grupos de clientes, mas com proporções diferentes. Essas técnicas permitiu a identificação de grupos de clientes que possuem maiores balanços (dinheiro guardado para realizar compras), maiores valores de compras e maiores valores de compras a prazo.

**Auto ML detecção de anomalias (PyCaret)**: Nesse projeto utilizo a biblioteca *PyCaret* identificar anomalias em uma base de cartões de créditos e depois analisar se as anomalias identificadas são ou não fraudes. Foram aplicados três modelos (*Iforest*, *Histogram* e *PCA*) e dos modelos o que gerou um melhor resultado foi o *PCA*, pois 432 anomalias foram identificadas como fraudes (de um total de 492).

**Auto ML para previsão de preços de casas (TPOT)**: Aplicação da biblioteca *TPOT* para previsão de preços de casas. Nesse projeto utilizei 4 métodos de seleção de *features* (por correlação, por *Feature Importance* do modelo de árvore de regressão, por *RFE* e por *PCA*) e o modelo de melhor desempenho foi aquele cuja seleção foi via correlação. O modelo gerado foi um 

Os resultado podem ser vistos abaixo:

|Método de seleção de *features* | R^2     |  Erro absoluto médio  |  Erro quadrado médio|  Raiz do erro quadrado médio |  *MedAE* |  *R-squared* |
|:----------------:|:------------------:|:------------------:|:------------------:|:------------------: |:------------------:|:------------------:|
|**Correlação** | **3.173**| **2.558** | **10.071**|**0.025**|**2.193**|**70.3%**|
|*RFE* | 9.872| 8.558 | 97.447| 0.183 | 8.3|-7754.9%|
|*Feature Importance* | 10.477| 8.99 | 109.766| 0.2 | 9.219|-9522.3%|
|*PCA* | 11.747| 10.357 | 137.99| 0.253 | 11.693|-376.2%|

**AutoML para classificação de preços de celulares (TPOT)**: Aplicação da biblioteca *TPOT*

**Automatização de visualização de dados (AutoViz)**: Aplicação da biblioteca *AutoViz* para automatizar o processo de visualização de uma base de dados de carros usados. Foram gerados os gráficos *Scatterplot*, *Pairwise-plot*, Histograma, *Boxplots*, *QQplot*, *Violinplot*, *Heatmap*, *Pivot Table* e  *barplots* e, com esses gráficos, foi possíveis identificar:

1) a relação positiva entre a variável *engineSize* e o preço (*price*, variável alvo);

2) As variáveis contínuas não possuem uma distribuição normal, o que pode ser um problema na hora de passá-las para modelos de *machine learning* ou de *deep learning*, pois alguns desses modelos pressupõem normalidade nas variáveis e isso mostra que essas colunas precisam de algum tipo de tratamento (normalização ou padronização). Outra coisa que pode-se notar é a presença de muitos *outliers* na variável *price* que pode ser ruim para o treinamento de um modelo, então essa coluna pode requerer um tratamento.
