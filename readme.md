# Desafios IDwall - iddog

Aqui estão os desafios para a primeira fase de testes de candidatos da IDwall para as vagas de frontend e mobile (se você é front, acesse a pastinha de frontend; se você é desenvolvedor mobile, acesse a pastinha mobile)

Os requisitos mínimos para cada tipo de teste está no respectivo diretório.

Não há diferença de testes para diferentes níveis de profissionais, porém o teste será avaliado com diferentes critérios, dependendo do perfil da vaga.

1.  [Frontend](https://github.com/idwall/desafios-iddog/blob/master/frontend)
2.  [Mobile](https://github.com/idwall/desafios-iddog/blob/master/mobile)

## Como entregar estes desafios

Você deve criar um repositório para este projeto e fazer o _push_ no seu próprio repositório e enviar o link para _jobs@idwall.co_ ou para o email do recrutador, junto com seu LinkedIn atualizado.

Fique à vontade para adicionar qualquer tipo de conteúdo que julgue útil ao projeto, alterar/acrescentar um README com instruções de como executá-lo, melhrias de design, etc.

**Obs.:** Você não deve fazer um Pull Request para este projeto!

### 📃 Utilizar nossa API de cachorros :)

Todos os endpoints tem como base [`https://iddog-nrizncxqba-uc.a.run.app`](https://iddog-nrizncxqba-uc.a.run.app) e seguem a arquitetura REST utilizando JSON.

Todas as requisições devem ser encoded com Content-Type: application/json header. Pra todas as responses, incluindo erros, devem também utilizar REST com JSON.

### POST /signup

#### Sign/signup de usuário

```bash
POST /signup
```

```bash
curl "https://api-iddog.idwall.co/signup" \
-H "Content-Type: application/json" \
-d '{ "email": "your@email.com" }'
```

### GET /feed

#### Listas de cachorros

```bash
GET /feed
```

```bash
curl "https://iddog-nrizncxqba-uc.a.run.app/feed" \
-H "Authorization: $TOKEN" \
-H "Content-Type: application/json"
```

##### Queries

##### ?category

**Default**: `husky`<br/>
**Type**: `string`<br/>
**Options**: `husky`, `hound`, `pug`, `labrador`

## Carreira IDwall

Caso queira mais detalhes de como trabalhamos, quais são nossos valores e ideais, confira a página [Carreira IDwall](https://idwall.co/carreira) e mesmo que seu perfil não esteja listado nas vagas em aberto, lhe encorajamos a mandar seu CV! Valorizamos bons profissionais sempre e gostamos de manter contato com gente boa.

Boas implementações! 🎉
