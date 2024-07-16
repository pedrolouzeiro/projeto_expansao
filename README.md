# Expansão de uma Rede de Laboratórios

## Descrição do Projeto
Este projeto visa analisar dados e identificar as melhores localizações para a instalação de novos laboratórios de uma rede de medicina diagnóstica nos Estados Unidos. A análise exploratória dos dados e a modelagem preditiva foram realizadas para recomendar três ZIP codes ideais para essa expansão.

## Objetivo
O objetivo deste projeto é analisar dados demográficos, econômicos e transacionais para identificar os melhores locais para abrir novos laboratórios, levando em consideração fatores como demanda, características populacionais e econômicas.

## Dados Utilizados

    1. transacoes.csv - Registros de exames feitos por pacientes da rede em cada laboratório.
    2. testes.csv - Informações sobre os exames, como custo de aplicação e outras especificações técnicas.
    3. info_geo.csv - Informações sobre a localização de cada laboratório, incluindo endereço, latitude, longitude e ZIP code.
    4. economicos.csv - Dados econômicos relevantes a nível de ZIP code.
    5. demograficos.csv - Dados demográficos relevantes a nível de ZIP code.

## Metodologia
    O projeto foi realizado em três etapas principais:
    
    1. Tratamento e Limpeza dos Dados
    
      - Remoção de dados vazios e duplicados.
      - Conversão de tipos de dados para tipos apropriados.
      - Separação e mesclagem de tabelas utilizando o ZIP code como chave comum.
      
    2. Análise Exploratória de Dados
    
      - Análise de estatísticas descritivas e criação de novas features.
      - Foco em perguntas-chave para a definição de estratégias de expansão.
      - Criação de gráficos para visualização dos dados e suporte à tomada de decisões.
      
    3. Machine Learning
    
      - Definição de estratégia para encontrar locais sem laboratórios, com predominância de mulheres e idade mediana entre 28 e 40 anos, pois esses locais tendem a ser mais lucrativos.
      - Pré-processamento dos dados utilizando StandardScaler.
      - Utilização do algoritmo NearestNeighbors para encontrar os ZIP codes que atendem à estratégia definida.
      - Visualização das localizações dos 20 melhores locais e criação de um ranking dos 3 melhores ZIP codes.

## Ferramentas e Tecnologias
    - Linguagem de programação: Python
    - Bibliotecas: pandas, scikit-learn, Matplotlib, Seaborn, NumPy, pgeocode
    - Ambiente de desenvolvimento: Jupyter Notebook

## Resultados
Os três melhores ZIP codes para a instalação de novos laboratórios, com base na análise dos dados, são:

    92105 - San Diego, Califórnia
    85204 - Mesa, Arizona
    32210 - Jacksonville, Flórida
    
## Conclusão
Como se tratava de uma entrega rápida resolvi focar no mínimo de perguntas que faziam sentido para o projeto e com base nos dados e no público maioral foi definido uma única estratégia de expansão. A análise demonstrou que os ZIP codes 92105, 85204 e 32210 são os mais promissores para a expansão da rede de laboratórios, considerando a demanda e as características demográficas e econômicas da população. A implementação desses novos laboratórios pode aumentar a cobertura da rede e atender a uma maior demanda de pacientes.
