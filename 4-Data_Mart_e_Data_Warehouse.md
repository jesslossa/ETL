# Dicas para se criar um bom processo de ETL

Só carregar os dados, modificar quando necessário e gravar quando termina é a parte normal do processo. Entretanto, é importante ter alguns conceitos em mente na hora da criação do processo para evitar falhas ou retrabalhos.

## Disponibilidade das fontes de dados

As fontes (_raw data_, ou dados brutos) devem ser gravadas em locais seguros, de fácil acesso e com nenhuma, ou, se necessário, poucas alterações na estrutura.

Sempre que possível procure trabalhar com bases homologadas pela empresa (dados oficiais). Ao trabalhar com fontes de dados públicas é interessante verificar se sempre terá acesso aos dados.

## Periodicidade dos dados

É importante sempre definir os intervalos de tempo para que ocorram os processos de ETL, com base na necessidade das áreas de negócio ou do usuário. Geralmente, só temos essa informação de forma precisa depois de criar os processos uma primeira vez.

É importante sempre ter ciência dos tempos de carga (ou seja, quanto tempo leva para os pipelines de ETL serem processados, que deve ser considerado para a frequência e necessidade de atualizações), de quanto em quanto tempo os dados precisam de atualização e alinhar a expectativa de carga com a expectativa do usuário de negócio.

## Escalabilidade de dados

A tendência é que os dados somente cresçam e se acumulem, fazendo com que consuma cada vez mais recursos do sistema.

Isto deve ser pensado no momento da criação do modelo, deve-se entender o tamanho que vai chegar.

Dependendo deste tamanho a estratégia de atualização muda, será necessário criar rotinas quebradas com vários processamentos. Então para não ter surpresas e travamentos já pense nisto antes.

---

## Extensão do Aprendizado

Conforme dito, ETL é uma tecnologia e não uma ferramenta. Existem diversas ferramentas de ETL disponíveis no mercado, vamos citar algumas:

Baseadas em nuvem:

- Databricks
- Azure Data Factory
- AWS Glue
- Google Cloud Platform

Algumas outras:

- Microsoft Integration Services
- Oracle Data Integrator (ODI)
- IBM Information Server Data Stage
- Informatica Power Center

Cada uma dessas ferramentas tem suas particularidades, e diferentes formas de trabalho conforme suas regras internas e locais de operação.

## Mais conteúdos _online_ sobre ETL

- [Microsoft Learn - Extração, Transformação e Carregamento](https://learn.microsoft.com/pt-br/azure/architecture/data-guide/relational-data/etl)
- [O que é ETL? | Google Cloud](https://cloud.google.com/learn/what-is-etl?hl=pt-br#:~:text=ETL%20%C3%A9%20a%20sigla%20para,de%20dados%20ou%20data%20lake.)
- [O que é ETL? | Oracle Brasil](https://www.oracle.com/br/integration/what-is-etl/)
- [ETL: o que é e qual sua importância? - SAS](https://www.sas.com/pt_br/insights/data-management/o-que-e-etl.html)
- [O que é ETL? – Explicação sobre extrair, transformar e carregar - Amazon AWS](https://aws.amazon.com/pt/what-is/etl/)
- [O que significa ETL e como funciona? - Alteryx](https://www.alteryx.com/pt-br/glossary/etl)
- [ETL Pipeline - Introdução](https://www.youtube.com/watch?v=D5mwXMMA0e0&ab_channel=ProgramadorLhama) (vídeo - YouTube)
- [O que é ETL?](https://www.youtube.com/watch?v=FJz-pI_7Yeo&ab_channel=MindTek) (vídeo - YouTube)
