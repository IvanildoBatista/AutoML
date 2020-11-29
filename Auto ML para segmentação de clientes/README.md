# Sobre o projeto

Um dos grandes desafio de quem trabalha na área comercial de uma empresa é conseguir segmentar seus clientes, com a finalidade é otimizar recursos e estratégias para maximizar o lucro
da empresa, focando em grupos que possam ser prioritários e direcionar para eles mais serviços ou promoções. Existem várias técnicas para segmentação de clientes, mas o foco desse 
projeto e desviar das técnicas tradicionais de segmentação, principalmente por conta da base de dados utilizada. 

Nosso conjunto de dados possui 18 *features* o que torna bem mais desafiador o uso de métodos tradicionais de *clusterização*, por isso usarei o módulo de *cluster* da biblioteca
*PyCaret* com a finalidade de encontrar grupos de clientes que sejam similares. Uma outra vantagem dessa biblioteca é a quantidade baixa de código que será usada para gerar os 
resultados (*low code*).

Observação 1: Alguns gráficos dos resultados estão anexados na pasta *imagem*, pois não podem ser visualizados no *Github*.
Observação 2: Os modelos treinados encontram-se anexados.

## Resultados 

Foram aplicados três algoritmos de *clustering* (*K-Means*, *Agglomerative Clustering* e *Birch*) e todos os modelos geraram cada um quatro *clusters*, porém os grupos são
bastantes diferentes um dos outros em cada algoritmo.
