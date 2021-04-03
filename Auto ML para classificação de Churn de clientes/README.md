# *Auto-Sklearn* para previsão de *Churn*

Nesse projeto eu irei aplicar a biblioteca de *Auto Machine Learning Auto-Sklearn* para gerar um modelo que preveja o *Churn* de clientes de uma empresa de Telecomunicações.
A vantagem do processo de *Auto Machine Learning* é que todo processo de escolha, treinamento e *tunning* do modelo é algo automático, permitindo que tempo e esforço sejam aplicados 
para outras áreas do projeto. Além dessa biblioteca usarei algoritmos de reamostragem de dados para realizar o rebalanceamento das classes da variável alvo.

## O que é *churn* ?
Churn é uma métrica que indica o quanto uma empresa perdeu de receita ou clientes. Para calcular o churn, basta dividir a quantidade de clientes que perdeu até o final do período
pelo total de clientes que iniciaram. Exemplo: se você perdeu 10 clientes de 100 = 10% de churn rate. Essa métrica também usada em departamentos de pessoas para analisar a
rotatividade de funcionários de uma empresa em um determinado setor ou em toda a empresa.

## Etapas

1- Instalação de bibliotecas;

2- Importação das bibliotecas;

3- Importação da base de dados;

4- Análise Exploratória dos dados;

5- Transformações dos dados;

6- Modelagem dos dados (separação de dados de treino e teste, reamostragem dos dados, treinamento dos algoritmos e avaliação dos modelos);

7- Conclusão.

## Resultados

O melhor modelo foi o que utilizou a algoritmos de reamostragem *Instance Hardness Threshold* que obtive as melhores métricas de avaliação.
















