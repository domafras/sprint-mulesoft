# sprint-mulesoft
API de previsão do Tempo, capaz de:
- retornar dados traduzidos
- salvar localmente
- salvar na nuvem (FTP)
  

Projeto final desenvolvido durante a Sprint 6 do Programa de Bolsa da [Compasso UOL](https://compassouol.com/)

### Tecnologias
- [Anypoint Platform](https://anypoint.mulesoft.com/login/)
- [Anypoint Studio](https://www.mulesoft.com/platform/studio)
- [Postman](https://www.postman.com/downloads/)
- [000webhost](https://www.000webhost.com/)
- Organização da equipe:
  - [Trello](https://trello.com/)
  - [Teams](https://www.microsoft.com/pt-br/microsoft-teams/)
  - [Github](https://github.com/)

### Pré-requisitos

Antes de começar, você vai precisar ter em sua máquina os arquivos disponibilizados nesse repositório. 

Além do Java e uma IDE como [Anypoint Studio](https://www.mulesoft.com/platform/studio) em que você pode seguir esses passos:
```bash
1. 'Import'
2. Acessar 'Git'
3. Importar este repositório
4. Run 'api-previsao-do-tempo'
4. Guide com endpoint '/findPredictTimeWeek'
5. Utilizar Postman ou similar para enviar requisição
```
### Resumo
Passos que fizeram parte do desenvolvimento, desde a modelagem e configuração dos fluxos na plataforma Anypoint.

```bash
1. Criação da API Spec no Design Center
2. Publicação no Exchange
3. Importação da API ao Anypoint Studio
4. Requisição GET no Postman ('http://localhost:8081/findPredictTimeWeek')
    4.1 Retorno com os atributos traduzidos (ex.: date para data)
    4.2 Conversão de JSON para CSV
    4.3 Salvar 'arquivo.csv' localmente (configurar diretório)
    4.4 Salvar 'arquivo.csv' no FTP em nuvem (000webhost)
```

### Webhost
Para salvar o arquivo na nuvem via FTP, se faz necessário a configuração no site [000webhost](https://www.000webhost.com/).
```bash
No projeto, alterar arquivo 'properties.yaml' para correspondente à configuração nesse site
```

### Postman 
É através dele que se torna possível utilizar a API.

Ou seja, de fato retornar o conteúdo traduzido, gerar o arquivo em diretório local e salvar através do FTP na nuvem. 


```bash
Utilizando o método (GET)
```

### Endpoint:
```bash
(GET) /findPredictTimeWeek
# Apresenta a lista de condição do tempo de alguns dias
Acesse: http://localhost:8081/findPredictTimeWeek
```
### Cabeçalho:
```bash
Adicione ao Headers:

    - KEY cidade -> Pelotas
    - KEY estado -> RS
```
### Respostas:
```bash
Após clicar 'SEND' no Postman:

    1. Dados traduzidos no Body
    2. 'arquivo.csv' salvo em diretório configurado
    3. 'arquivo.csv' salvo na nuvem (FTP) configurado
```

---
### Contato e licença
Sem restrições ao uso, modificações e distribuição do código fonte.

Feito com ❤️ por [Leonardo Mafra](https://www.linkedin.com/in/leomafra/),  [Juliane Maran](https://www.linkedin.com/in/juliane-maran-168b73133/) e [William Bernardes](https://www.linkedin.com/in/williambernardesf/).
