# An Empirical Study on Quality Issues of eBay’s Big Data SQL Analytics Platform

Zhu, Feng; Xu, Lijie; Ma, Gang; Ji, Shuping; Wang, Jie; Wang, Gang; Zhang, Hongyi; Wan, Kun; Wang, Mingming; Zhang, Xingchao; Wang, Yuming; Li, Jingpin. "An empirical study on quality issues of eBay's big data SQL analytics platform" in *Proceedings of the 44th International Conference on Software Engineering (ICSE-SEIP '22)*, pp. 33-42, 2022\. doi: [10.1145/3510457.3513034](https://doi.org/10.1145/3510457.3513034)

## 1\. Fichamento de Conteúdo

O artigo apresenta uma análise abrangente das questões de qualidade de serviço na plataforma de análise SQL de big data da eBay, chamada Carmel, que é baseada em Apache Spark. O contexto se insere na crescente adoção de soluções de código aberto para análise de dados, que, embora populares, carecem de estudos empíricos sobre a qualidade do serviço. O problema central que o artigo aborda é a identificação e análise das falhas comuns encontradas durante a execução de consultas, as quais impactam a experiência dos usuários e a eficiência operacional. Para isso, os autores realizam um estudo empírico que examina 1.884 problemas reais relacionados à qualidade do serviço em um período de um ano, utilizando dados coletados a partir do sistema JIRA da eBay e outras ferramentas de monitoramento. Os resultados revelam sintomas frequentes de falhas e suas causas raiz, fornecendo insights valiosos que podem ser aplicados para mitigar problemas similares em outras plataformas. Além disso, o artigo sugere direções para futuras pesquisas e o desenvolvimento de ferramentas automatizadas que possam facilitar a manutenção e a evolução dos sistemas de análise de dados, destacando a relevância das adaptações necessárias em face das características dinâmicas dos dados e dos workloads que os sistemas enfrentam.

## 2\. Fichamento Bibliográfico 

* **Qualidade de Serviço em Plataformas de Big Data**: A qualidade do serviço em plataformas de análise SQL de big data é crucial para a experiência do usuário e a operação eficiente do sistema (página 7).

* **Metodologia de Estudo Empírico**: A pesquisa analisou 1.884 problemas reais na plataforma Carmel usando o sistema JIRA e logs de auditoria, fornecendo dados detalhados sobre falhas (página 1).

* **Causas Raiz das Falhas**: As falhas são causadas por defeitos internos, incompatibilidades entre componentes e erros do usuário, essenciais para melhorar a confiabilidade (página 1).

* **Oportunidades de Pesquisa Futuras**: Surgem oportunidades de pesquisa em detectores automáticos de anti-padrões SQL e melhorias nas transformações de planos de consulta (página 9).

* **Dificuldades na Reprodutibilidade de Problemas**: A arquitetura elástica, como o YARN, torna difícil reproduzir e diagnosticar problemas, dificultando a resolução pelas equipes de engenharia (página 9).

## 3\. Fichamento de Citações 

* "We present the first comprehensive study on service quality issues of open-source based big data SQL analytics platform."

* "Carmel has been serving thousands of customers from hundreds of teams globally for more than 3 years."

* "We analyze 1,884 real-world service quality issues occurred on Carmel in a whole year."

* "There are about 20% of system issues that can be attributed to the architecture design limitations of Spark’s internal components."

* "An automatic and intelligent anti-pattern detector can free both users and engineers from these pain points."

* "Our work can not only help alleviate the pains in big data platform maintenance, but also inspire research interests and motivate candidate research directions."