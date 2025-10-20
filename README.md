## Links para baixar os dados trabalhados no projeto
### link para selecionar, de maneira simples, os nomes dos candidatos por local desejado

[Prestação de contas dos candidatos - TSE](https://divulgacandcontas.tse.jus.br/divulga/#/home)

Clica no mapa da região desejada, no campo *Consultas por Regiões Brasileiras*

Copiar os nomes na página da prestação de contas do TSE, foi a maneira mais simples que encontrei de relacionar os nomes completos dos candidatos e seus respectivos codinomes utilizados na campanha, para filtrar no arquivo dos dados eleitorais dos candidatos.

### link do TSE para baixar os dados dos candidatos por estado
[Número de votos por seção - TSE](https://dadosabertos.tse.jus.br/dataset/resultados-2024)


### link do TSE para baixar os dados dos eleitores por estado
[Perfil do eleitor - TSE](https://dadosabertos.tse.jus.br/dataset/eleitorado-2024)

### link com os endereços dos locais de votação
[Lista de ruas e seus respectivos CEPs](https://simoesfilho.ba.gov.br/wp-content/uploads/2024/05/CEP-SIMOES-FILHO-1.pdf)

*Converti o arquivo pdf para xlsx, utilizando algum conversor aleatório, e depois para CSV, utilizando o Google Planilhas*

## Separação por entidades

- CANDIDATO
  - ID_CANDIDATO
  - DS_CARGO
  - NR_VOTAVEL
  - NM_CANDIDATURA
  - SQ_CANDIDATO
  - ANO_ELEICAO
  - NM_VOTAVEL

- VOTOS_SECAO
  - ID_VOTOS_SECAO
  - ID_CANDIDATO
  - ID_LOCAL_VOTACAO
  - NR_SECAO
  - QT_VOTOS

- LOCAL_VOTACAO
  - ID_LOCAL_VOTACAO
  - NM_BAIRRO
  - NM_CIDADE
  - NR_CEP
  - NM_LOCAL_VOTACAO
  - DS_LOCAL_VOTACAO_ENDERECO

* Preciso criar um campo com o local ao qual pertencem os candidatos e o turno das votações
* Preciso de um arquivo com informações dos bairros, das cidades e dos CEPs pertencentes aos locais de votação

## *NOTA!!*
Estou reagrupando as colunas do arquivo principal para criar entidades, durante o processo, encontrei registros de outros municípios.

O problema citado acima ocorreu por causa da estratégia de isolar apenas registros de Simões Filho tomando como base os nomes completos dos candidatos. Até o momento, foi percebido que pelo menos 2 candidatos de outros municipíos tiveram seus registros incluídos no arquivo em questão.

A hipótese mais plausível é que existam candidatos, de municípios diferentes, que tenham exatamente o mesmo nome.

No momento, a estratégia que será adotada para contornar o problema, será filtrar quais os registros de votos têm seus endereços pertencentes ao município de Simões Filho - BA.