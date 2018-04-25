# Desafio IDwall - Frontend

<img src="https://github.com/idwall/desafios-iddog/blob/master/frontend/media/id-dog.gif?raw=true" />

## Objetivos do desafio

Com este desafio, esperamos aprender os seguintes pontos sobre seu trabalho:

* Como é seu estilo de trabalho e código
* Como é sua organização para o projeto
* Qual é o seu estágio atual de conhecimento sobre as ferramentas requeridas

## Stack a ser utilizada

* React e Redux (obrigatórios)
* Testes (componentes, actions, reducers etc), Linter

Você pode utilizar os plugins e packages que achar necessários para a realização do desafio.

## Instruções

Esperamos que você crie uma aplicação que capture os dados da [API do IDdog](https://iddog-api.now.sh), e apresente numa interface cumprindo os itens abaixo.
**Dica:** Utilize o GIF da introdução como inspiração para as interações e etapas do desafio. Mas não precisa aplicar o mesmo style, sinta-se livre para criar como quiser neste aspecto.

### Página de Signup

* Crie uma página `/signup` com um campo de email, e autentique o usuário postando apenas seu email no [endpoint de autenticação](https://iddog-api.now.sh/signup).
* A chamada na API retornará um `token` JWT, que deverá ser armazenado (cookie, localStorage) para ser utilizada nas chamadas seguintes.
* Após receber e armazenar o `token`, redirecione para a página de `/feed`. Caso o usuário acesse novamente o endereço `/signup` e tenha um `token` válido, ele deverá ser redirecionado automaticamente para a página de `/feed`.
* Caso um usuário tente acessar quaisquer das demais rotas, e não tenha o `token` salvo localmente, este deverá ser redirecionado automaticamente para a página de `signup`.
* Caso quaisquer das requisições das etapas seguintes sejam recusadas por conta do `token` ser inválido, o usuário deverá ser redirecionado automaticamente para a tela de `/signup`, com um aviso de "Sessão expirada".

### Página de Feed

* A página de `/feed` deverá ter 4 rotas - `husky`, `labrador`, `hound` e `pug`, e deverá ser acessível apenas se o `token` estiver salvo localmente.
* Cada rota, ao ser clicada, deve realizar uma chamada `GET` no [endpoint do feed](https://iddog-api.now.sh/feed), com seu respectivo parâmetro de `category`, [conforme este exemplo](https://your-website.com/feed?category=labrador).
* O resultado dessa requisição deverá ser apresentado na interface, conforme o exemplo do gif introdutório.
* Ao carregar a página de `/feed`, deverá ser feita uma chamada `GET` no [endpoint do feed](https://iddog-api.now.sh/feed). Essa chamada corresponde à mesma chamada para a categoria `husky`. **Importante:** Para que estas chamadas funcionem corretamente, envie no `header` o parâmetro `Authorization` com o `token` previamente armazenado.
* A resposta dessa chamada inicial deve ser armazenada localmente para que, caso o usuário retorne para uma das rotas já previamente carregadas, uma nova requisição não seja necessária.

### Página de Foto

* Ao clicar em uma foto, a URL da página deve ser atualizada para `/feed?category=X&id=Y`, sendo `category` a categoria à qual aquela imagem pertence, e `id` o id da imagem recebido nas requisições anteriores.
* A foto deverá ser ampliada e destacada dos demais itens da página, com um overlay. 
* Ao clicar no overlay, a foto deverá desaparecer, e a URL retorna para `/feed?category=X`.
* Com a foto aberta, ao dar refresh na página, ela deverá retornar ainda aberta.

## Deploy

* Publique sua aplicação ([now](https://zeit.co/now) / [heroku](https://www.heroku.com/) / [netlify](https://www.netlify.com/)).
* Publique seu código no seu perfil no Github.
* Envie ambos os link de volta para seu contato com a IDwall.
