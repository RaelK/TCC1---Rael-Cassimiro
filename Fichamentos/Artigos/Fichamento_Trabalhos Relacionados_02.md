# Towards Comprehending Energy Consumption of Database Management Systems - A Tool and Empirical Study

**Referência completa:**  
Lella, Hemasri Sai; Chattaraj, Rajrupa; Chimalakonda, Sridhar; Manasa, Kurra. "Towards Comprehending Energy Consumption of Database Management Systems - A Tool and Empirical Study," in *Proceedings of the 28th International Conference on Evaluation and Assessment in Software Engineering (EASE)*, June 2024, Salerno, Italy. DOI: [10.1145/3661167.3661174](https://doi.org/10.1145/3661167.3661174)

## 1. Fichamento de Conteúdo

O artigo trata da crescente importância dos sistemas de gerenciamento de banco de dados (SGBDs) no contexto de eficiência energética. Diante da escassez de estudos na engenharia de software que abordem o consumo de energia desses sistemas, os autores propõem a ferramenta DBJoules, um software de código aberto que permite medir o consumo energético de consultas SQL e NoSQL. Foram realizados experimentos com MySQL, PostgreSQL, MongoDB e Couchbase, aplicando diferentes operações (SELECT, INSERT, UPDATE, DELETE, JOIN) sobre variados conjuntos de dados. Os resultados indicam que o consumo energético varia significativamente conforme o tipo de banco, a operação realizada e o contexto de uso. Não existe um SGBD que seja superior em todos os cenários, sendo necessária a análise dos requisitos específicos de cada aplicação. Além disso, fatores como arquitetura do sistema e tamanho do banco influenciam o desempenho energético. Apesar das limitações, como a dependência de versões e métodos de medição, o estudo fornece uma base empírica importante para escolhas mais sustentáveis em projetos de software que envolvem armazenamento e manipulação de dados.

## 2. Fichamento Bibliográfico

* A diversidade de bancos de dados influencia consideravelmente o consumo de energia durante as consultas (p. 9).
* A ferramenta DBJoules mede o consumo energético monitorando o uso de CPU e RAM durante a execução das consultas (p. 3).
* Operações padrão como SELECT, INSERT, UPDATE, DELETE e JOIN apresentam diferentes perfis de consumo energético dependendo do banco de dados utilizado (p. 9).
* Não existe um sistema de banco de dados que seja consistentemente mais eficiente energeticamente em todos os cenários, sendo necessária uma análise do contexto e requisitos específicos (p. 10).
* Variáveis como tamanho do banco, tipo de consulta e arquitetura do sistema impactam de forma significativa o consumo de energia (p. 8).
* Os resultados obtidos podem ser influenciados por versões específicas do software e configurações utilizadas, limitando a sua generalização (p. 8).

## 3. Fichamento de Citações

* "A escolha do sistema de banco de dados deve levar em consideração fatores como requisitos de usuário, tipo de dado e tamanho do dataset, pois nenhum sistema individual supera os demais em todos os aspectos de eficiência energética." (p. 10)
* "Nossos resultados empíricos revelam variações substanciais no consumo de energia entre diferentes sistemas de banco de dados e tipos de consultas." (p. 9)
* "A ferramenta proposta, DBJoules, facilita a medição do consumo de energia monitorando o uso de CPU e RAM durante a execução das consultas." (p. 3)
* "Consultas básicas como SELECT, INSERT, UPDATE, DELETE e JOIN foram analisadas para compreender seus perfis energéticos." (p. 9)
* "Variações no desempenho de acordo com versões do sistema e tamanhos de datasets podem influenciar significativamente os resultados de consumo energético obtidos na análise." (p. 8)
