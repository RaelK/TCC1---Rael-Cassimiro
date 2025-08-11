# Research on Automated Database Health Check and Slow SQL Optimization  

Tan, Xiaomin; Zhang, Yuzhong. "Research on Automated Database Health Check and Slow SQL Optimization" in *Proceedings of the 2024 International Conference on Cloud Computing and Big Data (ICCBD '24)*, pp. 294-299, 2024\. doi: [10.1145/3695080.3695132](https://doi.org/10.1145/3695080.3695132)

## 1\. Fichamento de Conteúdo 

O artigo aborda a otimização de desempenho de bancos de dados SQL, destacando a importância de identificar e resolver problemas de performance antes da implementação das consultas. O texto discute os desafios enfrentados devido à complexidade das operações de negócios e à variabilidade na habilidade dos desenvolvedores em escrever SQL eficiente. Para mitigar esses problemas, o artigo propõe a criação de uma biblioteca de regras baseada na lógica de negócios e o uso de modelos de linguagem avançados para analisar planos de execução ao longo do tempo. Métodos como análise de logs lentos, monitoramento em tempo real e previsão de tendências são empregados para fornecer uma solução abrangente de monitoramento e otimização de desempenho. Os resultados incluem a identificação de consultas SQL lentas e a previsão precisa de tendências de desempenho, permitindo uma intervenção proativa para manter a eficiência do sistema.

## 2\. Fichamento Bibliográfico 

* Desafios na Otimização de SQL (p. 294-295): A identificação de gargalos de desempenho em ambientes de alta concorrência e a variabilidade na habilidade dos desenvolvedores são destacados como principais desafios.

* Biblioteca de Regras (p. 296): A criação de uma biblioteca de regras baseada na lógica de negócios é proposta para abordar a degradação de desempenho de SQL.

* Análise de Consultas Lentas (p. 295-296): A extração e análise de consultas SQL lentas são realizadas para identificar padrões e propor otimizações.

* Monitoramento de Desempenho (p. 295): O monitoramento em tempo real de métricas como utilização de CPU e I/O é essencial para detectar e resolver problemas de desempenho.

* Previsão de Tendências (p. 296): Técnicas de segmentação de séries temporais e validação cruzada são usadas para prever tendências de desempenho e identificar consultas com desempenho decrescente.

## 3\. Fichamento de Citações 

* "To address the persistent issue of SQL performance degradation arising from repetitive business patterns, a rule library grounded in business logic has been meticulously assembled."

* "Slow SQL queries are extracted from logs, recording the execution user and duration time for each SQL."

* "Database performance are monitored in real time. Metrics include but not limited to CPU utilization, I/Os, the status of lock files and the total counts of connection."

* "Manually identifying differences in execution plans quickly is a daunting task. Thus, use of a Large Language Model(LLM) to analyze execution plans over time is crucial for drawing conclusions on SQL performance."

* "The detection of phrases such as 'increased cost,' 'higher memory consumption,' or 'longer execution times' in the conclusions will activate a warning system."