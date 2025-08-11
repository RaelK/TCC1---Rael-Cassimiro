# Predizendo os Vencedores dos Playoffs: Um Estudo de Caso com Aprendizado de Máquina em Partidas de Futebol Americano

**Referência completa:**  
Ponciano, Lesandro; Brasileiro, Francisco; Simpson, Robert; Smith, Arfon. "Predizendo os Vencedores dos Playoffs: Um Estudo de Caso com Aprendizado de Máquina em Partidas de Futebol Americano," em *Proceedings of the 38th Brazilian Symposium on Databases*, 7 páginas, sem data de publicação específica disponível no PDF.

## 1. Fichamento de Conteúdo

Este artigo apresenta um estudo empírico que utiliza algoritmos de aprendizado de máquina (AM) para prever os resultados dos playoffs na temporada de futebol americano. A pesquisa envolve coleta e raspagem de dados da web, seguida por um extenso processo de pré-processamento, incluindo imputação de valores ausentes, normalização e redução de dimensionalidade por meio de seleção de atributos. O conjunto de dados resultante é dividido com a técnica de hold-out (80% treino, 20% teste), e diferentes algoritmos são treinados e avaliados utilizando métricas como acurácia, precisão, F1-score, entre outras. A pesquisa também incorpora a análise temporal da evolução das equipes, o que enriquece a qualidade preditiva dos modelos. Os resultados destacam a importância do pré-processamento e da escolha de atributos para a performance dos modelos. O estudo contribui com uma abordagem validada para uso de AM na previsão de resultados esportivos, com possíveis aplicações em análise de desempenho esportivo e estratégias de apostas. A metodologia empregada é robusta, com análise quantitativa e empírica bem definida, consolidando o trabalho como relevante no campo da engenharia de software aplicada a sistemas de dados e aprendizado automatizado.

## 2. Fichamento Bibliográfico

* Após o pré-processamento, a redução de dimensionalidade foi realizada principalmente por técnicas de seleção de atributos, que apresentaram melhores resultados do que a extração de atributos (p. 4).
* O método de hold-out foi utilizado para dividir os dados em conjuntos de treino (80%) e teste (20%) (p. 5).
* Para avaliação dos modelos, foram empregadas métricas como acurácia, acurácia balanceada, precisão, recall e F1-score, possibilitando uma análise completa do desempenho (p. 5).
* Os experimentos também incluíram análises de evolução temporal dos times, permitindo compreender melhor o comportamento dos modelos ao longo da temporada (p. 5).
* Técnicas simples de imputação, como média para valores numéricos e moda para categóricos, foram usadas na limpeza dos dados, além de normalizações baseadas em quartis e mediana para maior robustez contra outliers (p. 4).
* Os resultados detalhados e comparativos dos algoritmos estão apresentados na Tabela 2, destacando o desempenho de diferentes modelos na previsão dos resultados (p. 5).

## 3. Fichamento de Citações

* "Para que o processamento do algoritmo de AM não seja tão complexo, devido à existência de um alto número de atributos, foi utilizada a redução de dimensionalidade, cujo objetivo é diminuir a dimensão dos dados, eliminando atributos irrelevantes ou redundantes." (p. 4)
* "A avaliação dos modelos foi realizada com métricas que incluem acurácia, acurácia balanceada, precisão, recall e F1-score." (p. 5)
* "Considerando a evolução das equipes durante a temporada, foi possível realizar análises temporais que aprimoram a previsão dos resultados." (p. 5)
* "A divisão dos dados em conjuntos de treino e teste foi feita por meio do método hold-out, em proporções de 80% para treino e 20% para teste." (p. 5)
* "Técnicas simples de imputação, como a média e a moda, foram utilizadas na limpeza dos dados, além de normalizações baseadas em quartis e mediana." (p. 4)
