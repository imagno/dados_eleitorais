### link para selecionar, de maneira simples, os nomes dos candidatos por local desejado
#### Clica no mapa da região desejada, no campo *Consultas por Regiões Brasileiras*
https://divulgacandcontas.tse.jus.br/divulga/#/home

Copiar os nomes na página da prestação de contas do TSE, foi a maneira mais simples que encontrei de relacionar os nomes completos dos candidatos e seus respectivos codinomes utilizados na campanha, para filtrar no arquivo dos dados eleitorais dos candidatos.

### link do TSE para baixar os dados dos candidatos por estado
https://dadosabertos.tse.jus.br/dataset/resultados-2024


### link do TSE para baixar os dados dos eleitores por estado
https://dadosabertos.tse.jus.br/dataset/eleitorado-2024

### link com os endereços dos locais de votação
**PESQUISANDO**

### Separação por entidades

- CANDIDATO
  ID_CANDIDATO
  DS_CARGO
  NR_VOTAVEL
  NM_CANDIDATURA
  SQ_CANDIDATO
  ANO_ELEICAO
  NM_VOTAVEL

- VOTOS_SECAO
  ANO_ELEICAO
  ID_CANDIDATO
  ID_LOCAL_VOTACAO
  NR_SECAO
  QT_VOTOS

- LOCAL_VOTACAO
  ID_LOCAL_VOTACAO
  NM_BAIRRO
  NM_CIDADE
  NR_CEP
  NR_SECAO
  NM_LOCAL_VOTACAO
  DS_LOCAL_VOTACAO_ENDERECO

* Preciso criar um campo com o local ao qual pertencem os candidatos e o turno das votações
* Preciso de um arquivo com informações dos bairros, das cidades e dos CEPs pertencentes aos locais de votação