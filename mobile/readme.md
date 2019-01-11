# Challenge for Mobile (Android and iOS) Developers

Crie um aplicativo para Android (Kotlin ou Java) ou iOS (Swift ou Object C) com as seguintes características:

* Criar uma tela de login onde o usuário precisa digitar um endereço de email válido.
* Armazene localmente o token retornado pela API no login.
* Após o login feito com sucesso, redirecione para uma tela onde deve conter as listas com as imagens
* Crie uma forma para que o usuário possa navegar entre as quatro raças de cachorros (`husky`, `labrador`, `hound` e `pug`)
* Ao clicar em uma imagem, ela deve ser exibida de forma expandida.

[doc da API](https://github.com/idwall/desafios-iddog)

## Requisitos técnicos

* Fazer cache das imagens
* Versão mínima: Android API 16 ou iOS 9
* É recomendado o uso de libs de terceiros para:
  * chamadas de rede
  * download e cache das imagens
* O uso de todas as libs deve ser justificado no `README`.
* Faça um `README` documentando tópicos que julga importante para quem for avaliar, tais como arquitetura, libs, decisões, como executar o projeto, etc.
* Caso tenha desenvolvido para Android, disponibilize o `.apk`.

## Avaliação

* Arquitetura utilizada
* Boas práticas de layout
* Qualidade do código
* Uso de libs
* Uso do git
* Testes unitários/instrumentados
* Tratamento de erros
