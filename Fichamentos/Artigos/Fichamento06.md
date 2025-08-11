# Caracterização de Estratégias de Futebol com base na Frequência, Importância e Efetividade de Jogadas 

Valadao, Gabriel; Gonçalves, João L. L.; Megale, João L. L.; Paula, Vinicius M.; Rios-Neto, Hugo; Pereira, Adriano C. M.; Meira Jr., Wagner. "Caracterização de Estratégias de Futebol com base na Frequência, Importância e Efetividade de Jogadas" in *Anais do XX Encontro Nacional de Inteligência Artificial e Computacional (ENIAC 2023\)*, 2023\. doi: [10.5753/eniac.2023.234936](https://doi.org/10.5753/eniac.2023.234936)

## 1\. Fichamento de Conteúdo 

O artigo aborda a análise de estratégias no futebol, focando na identificação de jogadas frequentes, importantes e efetivas. Valadao et al. propõem uma metodologia que visa superar as limitações de estudos anteriores que se concentravam apenas em passes, negligenciando outras ações relevantes. A metodologia emprega agrupamentos do método SoccerMix e estimativas do arcabouço VAEP para uma análise mais abrangente das ações das equipes. Os resultados demonstram a eficácia da abordagem na caracterização de diferentes estilos de jogo, ressaltando a importância de dados detalhados das partidas para aprimorar a tomada de decisões e o desenvolvimento de estratégias. A pesquisa destaca a relevância de combinar diferentes métricas para uma compreensão mais profunda das estratégias de futebol, considerando a complexidade inerente ao esporte e a necessidade de equilibrar frequência, importância e efetividade das jogadas.

## 2\. Fichamento Bibliográfico 

* Dados de Eventos e SPADL: Utilização de dados de eventos de partidas de futebol, convertidos para a representação SPADL (Soccer Player Action Description Language) para padronizar as taxonomias e atributos e facilitar a análise (página 6).

* Enriquecimento das Ações: As ações são enriquecidas com informações de localização (através de grade ou SoccerMix) e potencial ofensivo (VAEP), permitindo uma análise mais detalhada e contextualizada (página 6).

* SoccerMix: Utilização do SoccerMix para agrupar ações com base em localização e direção, possibilitando a representação probabilística de ações do jogo (página 7).

* VAEP (Valuing Actions by Estimating Probabilities): O VAEP é utilizado para valorar as ações dos jogadores, estimando a probabilidade de marcar ou sofrer um gol como resultado de uma ação (página 8).  
* Construção de Jogadas: As jogadas são construídas como sequências de ações contíguas executadas pelo mesmo time, incluindo passes, cruzamentos, conduções, dribles e chutes (página 8).

* Mineração de Sequências Frequentes: A mineração de sequências frequentes é utilizada para identificar padrões nas jogadas, com o suporte sendo a medida de frequência mínima (página 9).

## 3\. Fichamento de Citações 

* "Estratégia de futebol é definida como um conjunto de jogadas que devem ser frequentes, importantes e efetivas, que são critérios normalmente conflitantes".

* "No domínio da análise de dados no futebol, os dados de eventos desempenham um papel crucial, fornecendo informações detalhadas sobre os eventos que ocorrem durante as partidas, como passes, dribles, chutes, faltas, cartões, substituições, início e fim de tempo, entre outros".

* "Para tentar solucionar essas limitações, este trabalho propõe uma nova abordagem para a construção de jogadas e a filtragem de jogadas consideradas como oportunidades de gol".

* "O objetivo deste trabalho é qualificar e quantificar jogadas típicas dos times e sua efetividade, como uma forma de sintetizar as estratégias e auxiliar no processo de aperfeiçoamento tático, tanto de ataque quanto de defesa".

* "Um dos desafios da caracterização de estratégias de futebol é identificar as estratégias típicas de cada time, representada por jogadas ou partes de jogada relevantes sob um ou mais critérios".

* "Utilizando dados reais, foi possível avaliar diferentes aplicações da metodologia proposta, na qual a escolha do SoccerMix se mostrou valiosa em relação à grade para fins de agrupamento espacial das ações, oferecendo uma representação mais informativa e detalhada das estratégias dos times"