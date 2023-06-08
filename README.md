# Desafio Acelera Trilha 1 - Olist Brasil [07/06/2023]

Este repositório contém o projeto desenvolvido por Michel Souza Santana para o Desafio Acelera Trilha 1 da Olist Brasil, realizado em 7 de junho de 2023. O objetivo deste projeto é construir um Data Warehouse (DW) para a empresa Olist, permitindo obter insights de negócios mais precisos e relevantes a partir dos dados disponíveis.

## Fase 1: Transformação do ER em um BI usando ETL

Nesta fase do projeto, foi realizado o processo de Extração, Transformação e Carga (ETL) dos dados usando uma ferramenta local. O ETL é um processo utilizado para integrar dados de diferentes fontes, transformá-los em um formato analisável e carregá-los em um novo destino, como um data warehouse.

### O que é ETL?

ETL significa Extração, Transformação e Carga. É um processo utilizado para integrar dados de diferentes fontes, transformá-los em um formato adequado para análise e carregá-los em um destino específico, geralmente um data warehouse ou data lake. Os passos envolvidos em um processo ETL incluem:

1. Identificar as fontes de dados: Identificar as diferentes fontes de dados que serão utilizadas no processo de ETL, como bancos de dados, planilhas, arquivos CSV, feeds RSS, etc.

2. Extrair os dados: Extrair os dados das fontes identificadas, utilizando as ferramentas apropriadas para cada tipo de fonte. Por exemplo, bancos de dados podem ser extraídos usando SQL, enquanto planilhas podem ser extraídas usando bibliotecas como Pandas em Python.

3. Validar e limpar os dados: Após a extração dos dados, é importante validar e limpar os dados para garantir que estejam completos, precisos e consistentes. Isso envolve remover dados duplicados ou inválidos, preencher valores ausentes e corrigir quaisquer inconsistências.

4. Transformar os dados: Os dados extraídos podem precisar passar por transformações para se adequarem ao formato desejado no destino. Isso pode incluir a conversão de tipos de dados, a criação de novas colunas, a agregação de dados, entre outros.

5. Analisar os dados: Após a transformação dos dados, é possível realizar uma análise exploratória para entender melhor os dados, identificar padrões, criar gráficos e aplicar técnicas de análise.

6. Selecionar recursos: Nem todos os dados são relevantes para o problema em questão. É importante selecionar os recursos mais importantes para o modelo ou análise que está sendo desenvolvida.

7. Dividir os dados: Antes de construir o modelo final ou realizar análises mais aprofundadas, é comum dividir os dados em conjuntos de treinamento e teste. O conjunto de treinamento é usado para desenvolver o modelo, enquanto o conjunto de teste é usado para avaliar sua precisão.

8. Verificar qualidade: Após a divisão dos dados, é importante verificar a qualidade dos mesmos para garantir que estejam prontos para uso. Isso inclui a identificação de valores ausentes, inconsistentes ou anômalos, além de validar as distribuições das variáveis.

9. Preparar dados para o modelo: Pre...ização, enriquecimento e agregação de dados. Nesta etapa, serão aplicadas técnicas de limpeza e validação dos dados, como remoção de valores duplicados, preenchimento de valores ausentes, padronização de formatos, entre outras. Além disso, serão realizadas transformações nos dados para torná-los mais adequados para análise, como a conversão de tipos de dados, criação de colunas derivadas e agregações.

Após o processamento e transformação dos dados, eles serão armazenados na camada de dados refinados (refined data layer), prontos para serem utilizados na análise e na construção de visualizações.

    • Sistemas de consulta e análise: Nesta etapa, os dados refinados serão disponibilizados para consulta e análise. Serão utilizadas ferramentas e técnicas de análise de dados, como SQL, OLAP (Processamento Analítico Online) e data visualization (visualização de dados). Essas ferramentas permitirão explorar os dados, realizar consultas complexas, criar relatórios e visualizações interativas para comunicar as descobertas de forma clara e eficaz.

A arquitetura proposta visa atender às necessidades de um projeto de construção de um Data Warehouse (DW) para a empresa Olist, permitindo a integração, processamento e análise dos dados do comércio eletrônico no Brasil. A utilização de pipelines de ingestão de dados, armazenamento em camadas e sistemas de consulta e análise proporciona uma abordagem escalável, eficiente e flexível para lidar com volumes de dados crescentes e complexidade das análises.

Além disso, a arquitetura contempla a utilização de tecnologias e ferramentas adequadas para cada etapa do processo, como ferramentas de ETL para a extração, transformação e carga dos dados, formatos de armazenamento otimizados como o Parquet, e ferramentas de consulta e análise de dados.

Requisitos de instalação e configuração:
Para reproduzir o projeto de construção do Data Warehouse (DW) para a empresa Olist, serão necessárias as seguintes ferramentas e tecnologias:

1. Ferramenta de ETL: Talend, Apache Hop, Nifi, Airflow, SSIS, Pentaho, ou outra ferramenta de ETL de sua preferência. Essa ferramenta será utilizada para realizar a extração, transformação e carga dos dados.

2. Ambiente de nuvem: Um ambiente de nuvem será necessário para hospedar o DW e executar as etapas do processo. Você pode utilizar provedores de nuvem como Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP) ou outras opções disponíveis.

3. Ferramenta de armazenamento de dados: Será necessário utilizar um sistema de armazenamento de dados adequado para a camada de dados refinados (refined data layer). Você pode optar por bancos de dados SQL, bancos de dados NoSQL, data lakes ou outras soluções de armazenamento compatíveis com suas necessidades.

4. Ferramentas de consulta e análise de dados: Serão necessárias ferramentas que permitam realizar consultas SQL, análises OLAP e criação de visualizações de dados. Existem diversas opções disponíveis, como bancos de dados analíticos, ferramentasde visualização de dados (por exemplo, Tableau, Power BI, QlikView, Plotly) e linguagens de programação para análise de dados (por exemplo, Python com bibliotecas como Pandas, NumPy e Matplotlib).

5. Plataforma de processamento distribuído: Dependendo do volume e da complexidade dos dados, pode ser necessário utilizar uma plataforma de processamento distribuído, como Apache Hadoop ou Apache Spark, para lidar com o processamento escalável e paralelo dos dados.

6. Recursos de segurança: É importante considerar recursos de segurança para proteger os dados armazenados no Data Warehouse. Isso inclui autenticação, controle de acesso, criptografia e monitoramento de atividades suspeitas.

7. Equipe de projeto: Para a implementação bem-sucedida do projeto, será necessário contar com uma equipe de profissionais qualificados, como engenheiros de dados, analistas de dados, arquitetos de dados e especialistas em visualização de dados.

É importante ressaltar que as ferramentas e tecnologias mencionadas são apenas algumas opções disponíveis, e a escolha pode variar de acordo com os requisitos específicos do projeto, o orçamento disponível e as preferências da equipe.

Além disso, ao implementar o Data Warehouse, é fundamental seguir boas práticas de projeto, como a modelagem dimensional, que permite a organização eficiente dos dados em esquemas estrela ou floco de neve, facilitando as consultas e análises.

Também é recomendável realizar testes de desempenho e monitoramento contínuo do Data Warehouse para garantir que ele atenda aos requisitos de escalabilidade, confiabilidade e desempenho esperados.

Em resumo, a construção de um Data Warehouse envolve a definição de uma arquitetura adequada, a seleção das ferramentas e tecnologias apropriadas, a implementação das etapas de extração, transformação e carga de dados, e a disponibilização dos dados para consulta, análise e visualização.
