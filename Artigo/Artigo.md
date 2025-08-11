# Análise de Tecnologias de Bancos de Dados para Geração de Registros em Tempo Real no Futebol

1. Rael Kiluanji de Jesus Cassimiro

* Orientador de conteúdo (TCC I): Joana Souza - joanasouza@pucminas.br 
* Orientador de conteúdo (TCC I): João Pedro Batisteli - jp.batisteli@hotmail.com
* Orientador de conteúdo (TCC I): Leonardo Vilela - leonardocardoso@pucminas.br 
* Orientador acadêmico (TCC I): Cleiton Tavares - cleitontavares@pucminas.br 

**Abstract.** 
This paper presents an experimental analysis of database technologies applied to the real-time generation of records in football. The objective is to identify which solutions offer the best technical performance to support applications that require continuous information updates, considering metrics such as latency, scalability, resource consumption, and operational cost. The research adopts an applied, quantitative, and experimental approach, performing controlled tests with different database management systems in simulated scenarios that represent the dynamics of event registration in professional football. The results allow comparing the performance of the evaluated solutions, identifying their limitations, and proposing guidelines for selecting the most suitable technologies for real-time record generation in the sports context.


**Resumo.** 
Este artigo apresenta uma análise experimental de tecnologias de bancos de dados aplicadas à geração de registros em tempo real no futebol. O objetivo é identificar quais soluções oferecem melhor desempenho técnico para suportar aplicações que exigem atualização constante de informações, considerando métricas como latência, escalabilidade, consumo de recursos e custo operacional. A pesquisa adota uma abordagem aplicada, quantitativa e experimental, conduzindo testes controlados com diferentes sistemas de gerenciamento de banco de dados em cenários simulados que representam a dinâmica de registros de eventos no futebol profissional. Os resultados permitem comparar o desempenho das soluções avaliadas, identificar suas limitações e propor diretrizes para a seleção de tecnologias mais adequadas à geração de registros em tempo real no contexto esportivo.

## Introdução

A análise de dados em tempo real tem ganhado destaque como estratégia essencial para apoiar decisões em diversos setores, incluindo o futebol profissional. O uso crescente de sensores embarcados, dispositivos vestíveis e plataformas de transmissão digital viabiliza a coleta contínua de dados durante partidas e treinamentos. Esses dados permitem ações como monitoramento de desempenho, prevenção de lesões e suporte a decisões táticas. Ponciano et al. [@ponciano2023nfl] ilustram a aplicação de algoritmos de aprendizado de máquina na previsão de resultados em competições esportivas. Valadão et al. [@valadao2023] exploram o uso de dados operacionais para caracterizar estratégias de jogo, com base na frequência e efetividade de jogadas. Já Calmon et al. [@calmon2024atletas] demonstram o potencial da integração de diferentes bases de dados na identificação de atletas promissores, indicando a importância de soluções eficientes de armazenamento e processamento.

Apesar dos avanços na coleta e armazenamento de dados esportivos, o uso analítico em tempo real ainda enfrenta desafios técnicos consideráveis. Limitações como alta latência nas consultas, consumo excessivo de recursos e baixa escalabilidade dificultam a aplicação prática desses dados em cenários de decisão rápida. Pesquisas recentes apontam que o desempenho das tecnologias de banco de dados varia significativamente conforme o contexto e a carga de trabalho [@rahman2024; @tan2024], demandando análises experimentais criteriosas. **O problema que esta pesquisa busca investigar é: quais tecnologias de banco de dados oferecem melhor desempenho técnico em contextos de análise de dados esportivos em tempo real, considerando métricas como tempo de resposta, escalabilidade e eficiência no uso de recursos?**

A relevância do problema proposto reside na crescente demanda por soluções que processem dados esportivos de forma eficiente, confiável e escalável. A análise precisa desses dados pode impactar diretamente o desempenho estratégico de equipes profissionais. Valadão et al. [@valadao2023] evidenciam que estratégias de jogo podem ser caracterizadas com base na frequência e efetividade das jogadas, desde que os dados sejam devidamente processados. Já Calmon et al. [@calmon2024atletas] demonstram que a integração de múltiplas bases e a aplicação de algoritmos de aprendizado de máquina podem prever o sucesso de jovens atletas, o que depende de infraestruturas de dados robustas. Essas evidências reforçam a necessidade de pesquisas que avaliem, sob condições controladas, o desempenho de diferentes tecnologias de banco de dados frente às exigências do cenário esportivo profissional.

**O objetivo geral deste trabalho é analisar criticamente e categorizar soluções de banco de dados aplicadas à análise de dados esportivos em tempo real no domínio do futebol.** Especificamente, busca-se identificar os principais requisitos técnicos relacionados ao desempenho e à escalabilidade que impactam a eficiência dessas tecnologias; examinar alternativas disponíveis na literatura sob a perspectiva da latência, confiabilidade e integração com sistemas analíticos; além de comparar essas soluções por meio de experimentos controlados, propondo diretrizes que orientem a seleção de tecnologias adequadas ao contexto futebolístico.

Como resultado, pretende-se apresentar uma categorização crítica das soluções de banco de dados para análise de dados futebolísticos em tempo real, considerando aspectos como desempenho em consultas, escalabilidade, confiabilidade e integração com sistemas analíticos.

O restante deste trabalho está organizado em três seções, além desta introdução. A Seção 2 aborda a fundamentação teórica, enquanto a Seção 3 trata dos trabalhos relacionados. A Seção 4 detalha os materiais e métodos adotados.

## 2. Fundamentação Teórica

A análise de dados em tempo real é fundamental para contextos que demandam monitoramento constante e suporte rápido à tomada de decisões. No esporte, especialmente no futebol profissional, a integração de dados provenientes de múltiplas fontes exige soluções robustas, escaláveis e eficientes, apoiadas por tecnologias de banco de dados, arquiteturas distribuídas e frameworks de integração de dados.

### 2.1 Banco de Dados em Tempo Real e Integração de Dados

Sistemas de gerenciamento de banco de dados (SGBDs) são essenciais para o armazenamento e processamento de dados em tempo real. A integração de dados históricos com dados em streaming permite consultas híbridas e análise contínua. Uma abordagem que possibilita essa integração é apresentada por meio de um framework que utiliza SQL como linguagem padrão, abstraindo as diferenças entre fluxos de dados e dados armazenados [amaral2021sqlintegration].

### 2.2 Arquiteturas Distribuídas e Monitoramento em Tempo Real

A utilização de arquiteturas distribuídas permite escalabilidade, baixa latência e alta disponibilidade, características indispensáveis em sistemas de monitoramento em tempo real. A integração entre sensores IoT, bancos de dados na nuvem e modelos preditivos oferece uma base sólida para aplicações que exigem atualização constante de informações e respostas rápidas [sinuraya2022wastemonitoring].

### 2.3 Dados Multimodais e Recuperação de Informação no Esporte

O volume crescente de dados esportivos — incluindo estatísticas, vídeos, imagens e dados de sensores — demanda soluções capazes de realizar consultas multimodais de forma eficiente. O projeto SoccerRAG propõe um framework que integra técnicas de Recuperação Aumentada por Geração (RAG) com Modelos de Linguagem de Grande Escala (LLMs) para permitir a recuperação de informações no contexto do futebol por meio de consultas em linguagem natural [strand2024soccerrag]. A arquitetura do SoccerRAG é composta por um banco de dados relacional estruturado, módulos de extração e validação de informações, além de um agente SQL que constrói consultas automáticas, garantindo respostas precisas a partir de bases multimodais que combinam dados tabulares, texto, vídeo e áudio.

### 2.4 Frameworks Adaptáveis na Análise Esportiva

O framework PlayField foi desenvolvido para enfrentar os desafios da integração de dados heterogêneos no domínio esportivo [pinto2024playfield]. Sua arquitetura modular permite mapear e transformar dados provenientes de diferentes formatos, como CSV, JSON e XML, em um modelo unificado, facilitando análises em larga escala. O PlayField conta com uma interface interativa para gestão de regras de transformação, além de uma API que automatiza o processo de integração de dados. Validado em parceria com a plataforma ZeroZero, o framework se destacou por sua capacidade de lidar com diferentes provedores de dados e adaptar-se rapidamente a mudanças nos esquemas, contribuindo diretamente para a eficiência das análises esportivas.

## Trabalhos Relacionados

Os trabalhos relacionados discutidos nesta seção envolvem o uso de bancos de dados e técnicas de análise de dados em tempo real, com ênfase em aplicações no domínio esportivo e em avaliações empíricas de desempenho e eficiência. Os estudos selecionados também abordam o uso de aprendizado de máquina em contextos similares. Dessa forma, os trabalhos estão organizados de acordo com o seu nível de aproximação com a proposta desta pesquisa, considerando tanto o objeto de estudo quanto a abordagem metodológica adotada.

Suh et al. [@suh2022gpu] realizaram um estudo empírico abrangente sobre o desempenho de consultas em sistemas de banco de dados baseados em GPU. Foram avaliados diferentes SGBDs utilizando benchmarks padronizados, considerando operações complexas como `JOIN` e agregações. Os autores empregaram um modelo causal para identificar os fatores mais impactantes no tempo de execução das consultas, revelando gargalos como a transferência de dados entre CPU e GPU e o uso limitado de memória da GPU. Este trabalho contribui para a presente pesquisa ao oferecer uma base metodológica sólida para comparação de desempenho entre SGBDs, especialmente úteis em aplicações de análise em tempo real, como o domínio esportivo explorado neste projeto.

Lella et al. [@lella2024energy] investigaram o consumo energético de sistemas de gerenciamento de banco de dados SQL e NoSQL, propondo uma ferramenta chamada *DBJoules*. O estudo avaliou operações típicas como `SELECT`, `INSERT`, `UPDATE`, `DELETE` e `JOIN`, em bancos como MySQL, PostgreSQL e MongoDB. Os resultados indicaram variações significativas no consumo de energia conforme a operação e a tecnologia utilizada. A presente pesquisa poderá se beneficiar dessas análises ao considerar aspectos de eficiência e sustentabilidade na escolha do SGBD mais adequado para aplicações esportivas com processamento em tempo real.

Ponciano et al. [@ponciano2023nfl] exploraram o uso de algoritmos de aprendizado de máquina para prever os vencedores dos playoffs da NFL. A abordagem envolveu coleta e preparação de dados históricos, aplicação de modelos como *Random Forest* e redes neurais artificiais, além da avaliação com métricas como *F1-score* e precisão. Os resultados demonstraram bom desempenho dos modelos e destacaram a importância de fatores como penalidades e jogadas ofensivas. Este trabalho serve como referência direta para a presente pesquisa, tanto na estrutura metodológica quanto na validação do uso de modelos de AM na previsão de eventos esportivos.

Calmon et al. [@calmon2024atletas] propuseram um modelo para prever o sucesso de jovens atletas de futebol com base em dados estatísticos. Foram utilizados algoritmos de classificação e seleção de atributos relevantes, visando identificar padrões associados a transições bem-sucedidas para níveis profissionais. A metodologia e o domínio de aplicação se aproximam diretamente da proposta desta pesquisa, fornecendo subsídios para estruturação de modelos preditivos voltados ao desempenho em jogos e análise de atletas.

Por fim, Souza e Oliveira [@souza2023comparacao] compararam os serviços Firebase e PostgreSQL com foco em critérios como desempenho, facilidade de uso e escalabilidade. Embora não seja um estudo empírico clássico, a análise técnica oferecida pelos autores é útil para fundamentar escolhas de infraestrutura de armazenamento em projetos com exigências específicas de resposta em tempo real. Esta comparação poderá ser considerada na definição da arquitetura do sistema proposto neste trabalho.

## Materiais e Métodos

A definição dos materiais e métodos empregados neste estudo está alinhada aos objetivos delineados na introdução e fundamentada nas contribuições discutidas nos trabalhos relacionados. A abordagem metodológica busca simular cenários típicos do domínio do futebol profissional, de modo a possibilitar a medição de desempenho de tecnologias de banco de dados sob condições equivalentes de uso.

### Tipo de Pesquisa

Este trabalho configura-se como uma **pesquisa aplicada**, voltada à resolução de problemas práticos relacionados à eficiência de tecnologias de banco de dados em aplicações esportivas. Trata-se também de um estudo **experimental**, pois envolve a execução de testes controlados em ambiente simulado. Adota-se uma abordagem **quantitativa**, focada na mensuração de variáveis objetivas de desempenho, e **descritiva**, ao buscar caracterizar o comportamento de diferentes soluções tecnológicas.

Essa combinação metodológica é coerente com a abordagem empregada por Suh et al. [@suh2022gpu], que conduzem experimentos com diferentes sistemas de gerenciamento de bancos de dados; por Lella et al. [@lella2024energy], que medem consumo energético de SGBDs; por Rahman et al. [@rahman2024], que analisam otimizações em SQL sob grande volume de dados; e por Tan e Zhang [@tan2024], que exploram desempenho de consultas em ambientes automatizados.

### Ambiente de Testes

Os experimentos serão realizados em um ambiente híbrido, composto por:

- **Infraestrutura computacional**: ambiente local e nuvem (AWS e Google Cloud) para simular diferentes cenários operacionais;
- **Sistema operacional**: Ubuntu Server 22.04 LTS, utilizado pela estabilidade e compatibilidade com os SGBDs e ferramentas empregadas;
- **Linguagem de programação**: Python 3.11, com bibliotecas específicas para acesso a bancos de dados, como `psycopg2`, `pymongo` e `sqlalchemy`;
- **Sistemas de gerenciamento de banco de dados (SGBDs)**: PostgreSQL (modelo relacional) [@souza2023comparacao], MongoDB (NoSQL orientado a documentos) [@calmon2024atletas], e Firebase (banco em tempo real).

A escolha desses recursos técnicos foi guiada por estudos prévios que demonstraram a relevância e aplicabilidade dessas ferramentas no contexto de dados esportivos em tempo real.

### Métodos Utilizados

Serão utilizados **benchmarks controlados e reprodutíveis**, simulando cargas de trabalho típicas de aplicações esportivas. A metodologia será estruturada em quatro eixos principais:

- **Consultas em tempo real**: baseadas em gargalos identificados por Tan e Zhang [@tan2024] e nos padrões de uso descritos por Valadão et al. [@valadao2023];
- **Requisições simultâneas e escalabilidade**: seguindo práticas observadas em Calmon et al. [@calmon2024atletas], com testes envolvendo crescimento de base de dados e variação de volume de dados;
- **Comparação entre tecnologias**: baseada na estrutura experimental proposta por Souza e Oliveira [@souza2023comparacao];
- **Eficiência energética**: utilizando métricas descritas por Lella et al. [@lella2024energy].

As bases de dados utilizadas serão públicas, com dados simulados inspirados em competições oficiais. Cada experimento será executado em três níveis de carga (10 mil, 100 mil e 1 milhão de registros).

### Métricas de Avaliação

As métricas adotadas neste estudo têm como base estudos anteriores [@rahman2024; @lella2024energy; @ponciano2023nfl] e foram selecionadas por refletirem exigências típicas de aplicações esportivas:

- **Tempo de resposta (ms)**: mede a latência média por tipo de consulta;
- **Taxa de sucesso (%)**: proporção de consultas concluídas sem falhas;
- **Consumo energético estimado**: monitorado com a ferramenta *DBJoules*;
- **Custo operacional por mil requisições**: estimado por meio de simulação em ambiente de nuvem;
- **Escalabilidade**: avalia a degradação de desempenho frente ao aumento de volume de dados.

Essas métricas refletem a necessidade de respostas rápidas e confiáveis em ambientes de tomada de decisão esportiva [@neto2023].

### Instrumentos Utilizados

Para a condução dos testes, serão utilizados:

- *Jupyter Notebooks* para orquestração e visualização de resultados;
- *DBJoules* para medição de consumo energético [@lella2024energy];
- *pgAdmin* e *Firebase Console* para administração de bancos;
- Scripts automatizados em Python para geração de carga e medição de desempenho.

### Cronograma de Execução

O cronograma da pesquisa está estruturado por quinzenas, abrangendo o período entre agosto e dezembro de 2025. As atividades previstas incluem levantamento de requisitos, implementação dos testes, execução dos experimentos e análise dos resultados.

| Etapa                               | Ago/1 | Ago/2 | Set/1 | Set/2 | Out/1 | Out/2 | Nov/1 | Nov/2 | Dez/1 | Dez/2 |
|------------------------------------|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|
| Levantamento de requisitos         |   X   |   X   |       |       |       |       |       |       |       |       |
| Configuração do ambiente           |       |   X   |   X   |       |       |       |       |       |       |       |
| Implementação dos scripts de teste|       |       |   X   |   X   |       |       |       |       |       |       |
| Execução dos experimentos          |       |       |       |   X   |   X   |   X   |       |       |       |       |
| Análise dos resultados             |       |       |       |       |       |   X   |   X   |   X   |       |       |
| Redação do capítulo de resultados  |       |       |       |       |       |       |   X   |   X   |   X   |   X   |


## Referências

[calmon2024]: Lucas Calmon, Rodrigo Ferro, Carlos Pereira, Caio Souza, Lucas Giusti, Glauco Amorim, Eduardo Ogasawara. *Previsão de Sucesso de Atletas Jovens de Futebol usando Integração de diferentes Base de Dados*. Anais do XXXIX SBBD, 2024. DOI: [10.5753/sbbd.2024.243187](https://doi.org/10.5753/sbbd.2024.243187)

[lella2024]: Hemasri Sai Lella, Rajrupa Chattaraj, Sridhar Chimalakonda, Kurra Manasa. *Towards Comprehending Energy Consumption of Database Management Systems: A Tool and Empirical Study*. Proceedings of the 28th International Conference on Evaluation and Assessment in Software Engineering (EASE), 2024. DOI: [10.1145/3661167.3661174](https://doi.org/10.1145/3661167.3661174)

[neto2023]: José dos Santos Neto, André Almeida Silva. *Estudo do Impacto da Adoção de Tecnologias Digitais no Futebol*. RECIMA21, v. 4, n. 3, 2023. DOI: [10.47820/recima21.v4i3.2923](https://doi.org/10.47820/recima21.v4i3.2923)

[ponciano2023]: Lesandro Ponciano, Francisco Brasileiro, Robert Simpson, Arfon Smith. *Predizendo os Vencedores dos Playoffs: Um Estudo de Caso com Aprendizado de Máquina em Partidas de Futebol Americano*. Anais do SBBD, 2023. DOI: [10.5753/sbbd_estendido.2023.232738](https://doi.org/10.5753/sbbd_estendido.2023.232738)

[souza2023]: Ismael Souza, Tiago Oliveira. *Comparação de Serviços de Banco de Dados na Nuvem: Amazon RDS vs Google Cloud SQL*. Anais do Simpósio Brasileiro de Sistemas de Informação (SBSI), 2023. DOI: [10.5753/latinoware.2024.245720](https://doi.org/10.5753/latinoware.2024.245720)

[rahman2024]: Md Mostafizur Rahman, Siful Islam, Md Kamruzzaman, Zihad Hasan Joy. *Advanced Query Optimization in SQL Databases for Real-Time Big Data Analytics*. Asian Journal of Business and Information Systems, v. 4, n. 3, 2024. DOI: [10.69593/ajbais.v4i3.77](https://doi.org/10.69593/ajbais.v4i3.77)

[suh2022]: Ah Reum Suh, Youhyun Wang, Hyunseok Jeong, Youngjae Lee, Jae-Gil Lee. *A Comprehensive Empirical Study of Query Performance Across GPUDBMSes*. Proceedings of the VLDB Endowment, v. 15, n. 9, 2022, p. 1842–1854. DOI: [10.14778/3529337.3529354](https://doi.org/10.14778/3529337.3529354)

[tan2024]: Xiaomin Tan, Yuzhong Zhang. *Research on Automated Database Health Check and Slow SQL Optimization*. Proceedings of the 2024 International Conference on Cloud Computing and Big Data (ICCBD '24), 2024. DOI: [10.1145/3695080.3695132](https://doi.org/10.1145/3695080.3695132)

[valadao2023]: Gabriel Valadão, João L. L. Gonçalves, João L. L. Megale, Vinicius M. Paula, Hugo Rios-Neto, Adriano C. M. Pereira, Wagner Meira Jr. *Caracterização de Estratégias de Futebol com base na Frequência, Importância e Efetividade de Jogadas*. Anais do XX ENIAC, 2023. DOI: [10.5753/eniac.2023.234936](https://doi.org/10.5753/eniac.2023.234936)

[amaral2021sqlintegration]: Amaral, J., Ströele, V., Braga, R., Dantas, M., & Bauer, M. (2021). *Stream and Historical Data Integration using SQL as Standard Language*. Anais do XXXVI Simpósio Brasileiro de Banco de Dados (SBBD). DOI: [10.5753/sbbd.2021.14334](https://doi.org/10.5753/sbbd.2021.14334)

[strand2024soccerrag]: Strand, A. T., Gautam, S., Midoglu, C., & Halvorsen, P. (2024). *SoccerRAG: Multimodal Soccer Information Retrieval via Natural Queries*. Proceedings of the 2024 International Conference on Content-Based Multimedia Indexing (CBMI). DOI: [10.1109/CBMI62980.2024.10859209](https://doi.org/10.1109/CBMI62980.2024.10859209)

[pinto2024playfield]: Pinto, F., & Lima, B. (2024). *PlayField: An Adaptable Framework for Integrative Sports Data Analysis*. Proceedings of the 2024 IEEE/ACM International Conference on Big Data Computing, Applications and Technologies (BDCAT). DOI: [10.1109/BDCAT63179.2024.00028](https://doi.org/10.1109/BDCAT63179.2024.00028)

[sinuraya2022wastemonitoring]: Sinuraya, E. W., Sumardi, Y. A. A., Soetrisno, Y. A., Setianingrum, A. P., Permata Sari, T. W. I., & Windarta, J. (2022). *Realtime Monitoring System Towards Waste Generation Management*. Proceedings of the 6th International Conference on Electrical, Telecommunication and Computer Engineering (ELTICOM). DOI: [10.1109/ELTICOM57747.2022.10038115](https://doi.org/10.1109/ELTICOM57747.2022.10038115)
