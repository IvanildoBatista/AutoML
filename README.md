# Sobre o repositório

Nesse repositório irá constar projetos onde foram aplicadas ferramentas e bibliotecas de *Auto Machine Learning*.

**Auto ML para modelar aluguéis**: Modelagem do preço de alugueis de casas e apartamentos no Brasil. Foi utilizada a biblioteca *PyCaret* para todas as etapas do projeto (tratamento, modelagem, avaliação, salvamento e carregamento); o modelo gerado foi um *Gradient Boosting Regressor* que obteve as melhores métricas de avaliação na validação cruzada. O R-squared do modelo foi de **0.9968**.

**Auto ML para identificação de risco de câncer**: Nesse projeto utilizo a biblioteca *PyCaret* para modelar dados de características de pacientes e suas biópsias, para identificar qual o risco de possuir ou não câncer cervical (ou do colo do útero). O modelo gerado foi um *CatBoost Classifier* com uma acurácia de **0.9419**.

**Auto ML segmentação de clientes**: Nesse projeto utilizo a biblioteca *PyCaret* gerar *clusters* (ou grupos) de clientes de uma empresa de cartão de crédito. Apliquei três algoritmos de *machine learning* que foram o *K-Means*, o *Agglomerative* e o *Birch*; e cada uma desses algoritmos gerou 4 grupos de clientes, mas com proporções diferentes. Essas técnicas permitiu a identificação de grupos de clientes que possuem maiores balanços (dinheiro guardado para realizar compras), maiores valores de compras e maiores valores de compras a prazo.



