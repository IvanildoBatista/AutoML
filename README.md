# Sobre o repositório

Nesse repositório irá constar projetos onde foram aplicadas ferramentas e bibliotecas de *Auto Machine Learning*.

**Projeto 1**: Modelagem do preço de alugueis de casas e apartamentos no Brasil. Foi utilizada a biblioteca *PyCaret* para todas as etapas do projeto (tratamento, modelagem, avaliação, salvamento e carregamento); o modelo gerado foi um *Gradient Boosting Regressor* que obteve as melhores métricas de avaliação na validação cruzada. Na validação do modelo obteve-se os seguintes resultados abaixo


|          |  Itens *X*  |   Item *Y*   |    Confiança    |     *Lift*      |
|:--------:|:-----------:|:------------:|:---------------:|:---------------:|
|Regra 1   | *cream cheese* e *domestic eggs*  |  *whole milk*|  0.71428    |   3.2117    |
|Regra 2   |*curd* e *domestic eggs*      |  *whole milk*      |  0.71428       |   3.2117   |
|Regra 3   | *domestic eggs* e *sugar*      | *whole milk*     |   0.7045       |      3.1679   |
|Regra 4   | *butter*, *other vegetables* e *whipped/sour cream*   | *whole milk*  | 0.723404 |  3.2527  |
|Regra 5   | *butter*, *other vegetables* e *yogurt*  |  *whole milk*  |  0.73469  |     3.3035  |
|Regra 6   | *citrus fruit*, *root vegetables* e *tropical fruit* |  *other vegetables*  |  0.8 | 4.7819  |


R-squared do modelo: 0.9968
Erro médio Absoluto do modelo: 96.011
Erro quadrado  médio do modelo: 37187.2977
Raiz do erro quadrado médio do modelo: 37187.2977
Raiz do logarítmo do erro quadrado médio do modelo: 0.0956
Erro percentual médio absoluto modelo: 0.0416
