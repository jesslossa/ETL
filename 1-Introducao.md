---
id: 666
tituloSuperior: Introdução ao ETL
tituloInferior: Conceitos básicos de ETL
---

# Introdução ao ETL

## Conceitos básicos de ETL

A sigla **ETL**, em inglês (**_Extract, Transform, Load_**), é o processo de **extração**, **transformação** e **carregamento** de dados. É uma forma tradicionalmente aceita para que as organizações combinem dados de vários sistemas em um único banco de dados, repositório de dados, armazenamento de dados ou data lake. O **ETL** pode ser usado para armazenar dados legados, ou, o que é mais comum, agregar dados para analisar e impulsionar decisões de negócios com base nesses dados.  

O **ETL** se trata um _conjunto de processos de dados_, portanto, não é um assunto que trata apenas sobre uma ferramenta específica. Muitas vezes é utilizado mais de uma ferramenta para implementar esses processos.

Para a definição de modelos de dados, o **ETL** é uma das fases mais importantes. Em um cenário de _BI_ (_Business Intelligence_), as fontes de dados necessárias para atender os requisitos de negócio podem ser as mais diversas, podendo existir até mesmo ter a possibilidade dos dados estarem distribuídos nos mais diversos sistemas e fontes.

> **Business Intelligence**:
>
> - _Business Intelligence_, ou _BI_, é o conjunto de estratégias e técnicas empregadas pelas empresas com o propósito de analisar dados e melhorar a tomada de decisão baseada em informações concretas. Como indica a sua tradução, é uma forma de proporcionar a inteligência para os negócios com base em dados.

É papel do **ETL** _extrair_ esses dados das respectivas fontes, _transformá-los_ (para obter padronizações e agregações) e _carregá-los_ em uma base de dados (podendo ser um _data warehouse_, ou banco de dados, repositório de dados, data mart, armazenamento de dados ou data lake de destino) que os reúna de forma centralizada. Assim, as ferramentas de _Data Visualization_ e usuários do negócio possuem acesso facilitado e rápido aos dados, ajudando a estabelecer um bom processo de _BI_.

> **Data Visualization**:
>
> - A visualização de dados é uma expressão contemporânea da comunicação visual, que consiste na representação visual de dados (em forma de gráficos, tabelas, KPIs e outros). No _Data Visualizaton_, há exibições gráficas que dão sentido aos dados, transformando-os em informações concretas. Exemplos de ferramentas de _Data Visualization_ mais utilizadas: _Power BI, Tableau, Qlik View_ e _Qlik Sense_. Podem também serem chamadas de ferramentas de _BI_.

## Aprofundando os conceitos de ETL

### "E" - _Extract_ (Extração)

A primeira etapa do processo é extrair os dados, que podem vir de diversas origens.

Dependendo da origem, os dados podem ter estruturas diferentes. Os dados também podem estar dispostos das mais diversas formas possíveis, dispostos de forma padrozinada ou não.

**Alguns exemplos de arquivos utilizados na extração:**

- Arquivos de Texto/CSV;
- Arquivos no formato Excel;
- Banco de Dados Relacionais;
- Banco de Dados alocados em Cloud;
- Bancos de Dados não relacionais (NoSQL, Graph Databases);
- Arquivos JSON e XML (por meio do consumo de APIs, principalmente);
- Conteúdos de endereços WEB;
- Arquivos em PDF;
- Arquivos tipo Blob (fotos, áudios, entre outros arquivos com dados brutos imutáveis).

A forma de extração pode ser completamente diferente entre os diferentes tipos de arquivos, devendo ser estabelecido um processo para cada um dos respectivos tipos, devido suas particularidades estruturais.

### "T" - _Transform_ (Transformação)

Consiste no tratamento e limpeza dos dados, provindos da etapa de extração.

Nesta fase, teremos várias etapas a fim de modelar os dados para a otimização das consultas realizadas pelos usuários dos dados.

A parte de transformação consiste, principalmente, em:

- Padronizar os dados em relação ao tamanho e tipo;
- Remover colunas ou linhas indesejadas;
- Substituir ou remover caracteres indesejados;
- Corrigir erros de digitação;
- Padronizar nomes e termos;
- Criação de novas colunas a partir de colunas já existentes, contendo somente parte dos dados (dependendo da necessidade do usuário);
- Criação de colunas a partir da junção e / ou mescla de duas ou mais colunas;
- Transposição de linhas para colunas, ou vice-versa;
- Traduzir valores codificados ou criptografados em informações legíveis (exemplo: 1 para "Verdadeiro", 0 para "Falso");
- Alteração das unidades de medida e / ou sistema de numeração decimal dos dados;
- Realizar operações de agregação dos dados, como, por exemplo, as operações em SQL _MAX_, _MIN_, _SUM_, _AVG_, _COUNT_ e _GROUP BY_;
- Mesclar ou acrescentar informações de várias tabelas em uma única tabela.

### "L" - _Load_ (Carregamento)  

O último processo consiste em armazenar esses dados já tratados em um modelo de Data Warehouse (geralmente, utilizando Modelagem Dimensional - para mais detalhes, verifique o curso aqui do ITC de _Introdução à Modelagem Dimensional_), para que esses dados possam ser utilizados e consultados pelos usuários, para fins de visualização e exploração destes.

> **Data Warehouse:**
>
> - Um _data warehouse_ é um tipo de sistema de gerenciamento de dados projetado para ativar e fornecer suporte às atividades de business intelligence (BI), especialmente a análise avançada. Os data warehouses destinam-se exclusivamente a realizar consultas e análises avançadas e geralmente contêm grandes quantidades de dados históricos. Os dados em um data warehouse geralmente são derivados de uma ampla variedade de fontes, como arquivos de log de aplicativos e aplicativos de transações.

A partir deste ponto, o analista ou gestor de negócios consegue manipular e formar seus relatórios e análises para o processos de tomada de decisões.
