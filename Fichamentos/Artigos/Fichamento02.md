# Research and Implementation of Complex Real-time Computing based on Data Middle Platform 

Wang, Peng; Li, Jiajin; Xuan, Baolong; Lu, Wei; Zhang, Xian; Hu, Jian; Yan, Hailang. "Research and Implementation of Complex Real-time Computing based on Data Middle Platform" in Proceedings of the IEEE Conference, pp. 1-10, Dec. 2023\. doi: [10.1109/EIECC60864.2023.10456691](https://doi.org/10.1109/EIECC60864.2023.10456691)

## 1\. Fichamento de Conteúdo 

O artigo analisa a crescente necessidade de processamento de dados em tempo real, particularmente no contexto de grandes volumes de dados. A complexidade das operações de dados tradicionais tem dificultado a tomada de decisões rápidas e acertadas nas empresas, levando à proposta de uma nova abordagem de cálculo em tempo real baseada em uma plataforma de dados. O método apresentado envolve a construção de tabelas dimensionais e de fatos incrementais, permitindo uma análise mais eficaz das mudanças nos dados empresariais sem depender excessivamente de operações de mesclagem de dados que consomem tempo. A eficácia da solução é validada através de aplicações práticas, como o cálculo em tempo real de contas de eletricidade, mostrando que a abordagem não apenas reduz o tempo de processamento, mas também melhora a precisão das estatísticas geradas. A pesquisa aponta que, embora o método tenha trazido melhorias significativas, ainda existem desafios a serem superados, como a necessidade de ainda mais velocidade nas respostas e a gestão de contenções de recursos.

## 2\. Fichamento Bibliográfico 

* **Plataforma de Dados Centraliza Processamento:** O artigo descreve a construção de uma "plataforma de dados central" que permite uma estrutura de dados unificada e serviços de dados externos consistentes (p. 1).

* **Necessidade de Tempo Real:** Com o aumento de demandas por dados em tempo real, o artigo destaca que a "o valor dos dados reside na sua temporalidade", ressaltando a importância de processar e utilizar dados prontamente (p. 2).

* **Modelagem Dimensional e Tabelas Incrementais:** A pesquisa discute a segmentação de dados em tabelas de fatos e dimensões, enfatizando a técnica de "modelagem dimensional" para facilitar análises mais precisas (p. 3).

* **Desafios de Cálculos em Tempo Real:** O texto menciona que "o processamento de dados em real-time é custoso e pode não suportar cenários complexos de lógica de negócios" (p. 4).

* **Resultados da Implementação Prática:** A validação do método através do "cálculo em tempo real de contas de eletricidade" indica sua aplicabilidade e eficácia em cenários reais (p. 6).

## 3\. Fichamento de Citações 

* "The value of data lies in its timeliness, if data is not processed and utilized promptly when generated, it cannot maintain the highest 'freshness' and maximize its value."

* "The current challenges that need to be addressed are as follows: How to achieve real-time statistics for daily data under the middle platform's offline batch processing architecture while ensuring the accuracy and timeliness of data statistics."

* "Dimensional modeling divides tables into fact tables and dimension tables based on the metrics in the business process and the context describing the business process." 

* "This real-time solution is built upon the full table and incremental table in the source layer of the offline system."

* "The complex real-time computing method proposed in this paper has been validated through the electricity charge calculations in JiangSu Energy Internet Marketing Service System Unified Software 2.0."

* "However, the current system still takes too long to generate metrics and does not achieve the capability for sub-second responses." 