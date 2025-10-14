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
[Lista de escolas públicas - INEP](https://anonymousdata.inep.gov.br/analytics/saw.dll?Portal&PortalPath=%2Fshared%2FCenso%20da%20Educa%C3%A7%C3%A3o%20B%C3%A1sica%2F_portal%2FCat%C3%A1logo%20de%20Escolas)

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
  - NR_SECAO
  - NM_LOCAL_VOTACAO
  - DS_LOCAL_VOTACAO_ENDERECO

* Preciso criar um campo com o local ao qual pertencem os candidatos e o turno das votações
* Preciso de um arquivo com informações dos bairros, das cidades e dos CEPs pertencentes aos locais de votação