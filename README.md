https://janarf.github.io/manchas-solares/

# Trabalho de Métodos Computacionais em Física 

## Análise Exploratória de Dados de Manchas Solares 

Trabalho final da disciplina: http://lilith.fisica.ufmg.br/~guerrero/fis045.html

Análise exploratória dos dados de manchas solares, visualização, análise estatística e aplicação de métodos clássicos a partir do livro: 

### Practical Time Series Analysis
Master Time Series Data Processing, Visualization and Modeling using Python

Dr. Avishek Pal, Dr. PKS Prakash


## Motivação

As manchas solares são a contagem de manchas na face visível do sol. Dados diários de sua contagem utilizando telescópios datam de 1610 e a partir de 1700 os dados são considerados consistentes para análise.

É possível perceber que as manchas estão relacionadas com o ciclo magnético do sol e são produzidas por um processo de dínamo hidromagnético. O modelo atual prevê dois dínamos acoplados.

Da mesma forma que em um dínamo eletromagnético temos uma espira rotacionando em um campo magnético temos um fluxo espiral de plasma (que também são bons condutores de calor) dentro do sol.

O sol apresenta atividade cíclica com duração média de 11 anos e amplitude variável. A importância dos dados de manchas solares fica evidente quando utilizados para modelar e prever a amplitude do próximo ciclo solar: previsões atuais são variada e contraditórias, variando de intensidade baixa até moderada.

Previsões da intensidade da atividade solar são importantes para agricultura, telecomunicações e astronomia entre outros.

A intensidade da atividade solar está diretamente relacionada com a incidência de UVB na superfície, quantidade de Ozônio formada na atmosfera, formação de nuvens e interferência na comunicação por ondas curtas.

## Objetivo

Fazer uma análise exploratória de dados para facilitar o desenvolvimento de um modelo preditivo eficiente para amplitude de ciclos.

A necessidade de feature design na análise de séries temporais se mostrou eficiente no artigo ["Clustering of Time Series Subsequences is Meaningless: Implications for Previous and Future Research"](http://www.cs.ucr.edu/~eamonn/meaningless.pdf). 
Assim, uma análise exploratória que faça tratamento prévio e selecione métodos adequados de predição de uma série temporal são essenciais para um modelo bem sucedido.

Neste trabalho, dados de manchas solares são visualizados e tratados de acordo com métodos estatísticos clássicos assim como é feita uma exploração utilizando Deep Learning. Ao final, sugerimos uma abordagem mista para a elaboração de modelos preditivos mais confiáveis.

## Tópicos abordados

- Capítulo 1: Introdução a Séries Temporais
    * Tipos de dados;
    * Estruturas internas de séries temporais: tendência, sazonalidade, movimentos cíclicos, variações inesperadas.
    * Modelos para análise de séries temporais: modelos de média zero, random walk, modelos de tendência, modelos de sazonalidade;
    * Autocorrelação e autocorrelação parcial;

- Capítulo 2: Entendendo os dados de uma série temporal
    * Processos estacionários;
    * Teste de Dickey-Fuller aumentado;
    * Métodos de decomposição de uma série temporal;
  
- Capítulo 3: Métodos baseados em suavização exponencial
- Capítulo 4: Modelos Autorregressivos

    **Modelos autorregressivos (AR)** são modelos estatísticos muitos bons em predição de séries temporais em que os valores seguintes dependem dos valores anteriores. Assim, modelos AR são muito utilizados na predição de séries temporais.
    * Modelo ARMA;
    
- Capítulo 5: Deep Learning para predição de série temporal

Chamamos de **deep learning** uma gama de métodos de aprendizado de máquinas mas o mais conhecido são as redes neurais com muitas *hidden layers*.

A arquitetura da rede neural deve ser adequada aos dados de entrada e saída, por exemplo: **redes neurais convolucionais (CNN)** são mais apropriadas para dados estruturados em 2D ou 3D (muito utilizada na classificação de imagens) enquanto **redes neurais recorrentes (RNN)** são utilizadas para modelos de análise de linguagem.

## Conclusões

As predições de curto prazo (1, 2 dias) tiveram erro baixo e foram bem sucedidas.

Não foi possível prever dados do próximo ciclo com as abordagem utilizadas mas o conhecimento de manipulação de séries temporais com métodos estatísticos podem ser aplicados a uma infinidade de outros dados disponíveis.

Uma abordagem diferente pode ser utilizar o modelo ARMA e o resíduo como entrada de uma rede LTSM autoenconding.


https://github.com/janarf/manchas-solares/blob/master/manchas%20solares/final-trabalhomanchassolares.ipynb
