## Sobre o teste

Para esse desafio vamos utilizar as API’s do Spotify.

 - Possibilidade de inserir o nome do artista ou de um album e retornar uma lista de albuns;
 - Quando retornado, o usuário poderá selecionar o album e será direcionado a lista de música desse album.
 - Tocar o preview da música.

### Requisitos básicos

- Você deve usar React;
- Você deve criar um repositório e compartilhar com a gente;
- Você não deve usar **scaffolds** (Create React App, etc.), queremos ver como você vai montar a estrutura do seu projeto;
- Quero conseguir rodar seu projeto rodando **yarn/npm** start;
- A aplicação deve solicitar o token que será utilizado para realizar as requisições para a API;
- Persistencia do **TOKEN**, quando expirado solicitar o token novo;

Nós usamos também redux, sei que não faz sentido para uma aplicação pequena mas seria legal para mostrar seus conhecimentos. Faz sentido, não?

### Visual & Funcionalidades

Quando o usuário entrar na aplicação ele deve poder buscar por um album ou artista. Quando realizar a busca ele deve conseguir ver todos os albuns do artista e pode interagir indo para a página do album, utilizando a url **/albums/{albumId}**, por exemplo: **/albums/552zi1M53PQAX5OH4FIdTx**. Ele deve conseguir voltar para essa página com o resultado da busca atual.

Quando estiver em uma tela de album ele deve ver as musicas e conseguir ouvir uma prévia da música que ele escolher, caso ele pause a música deve continuar de onde parou. Algum feedback para mostrar qual música está tocando seria legal.

### Telas

![](https://github.com/Mauricio32/challenger/blob/master/images/albumPage.jpg)

![](https://github.com/Mauricio32/challenger/blob/master/images/list.jpg)

Fique a vontade para fazer as mudanças de UI que achar necessário. =)

## Api

Você deve utilizar as API’s do Spotify. Sua aplicação deverá aceitar um TOKEN que o usuário passará para sua aplicação.

O link da documentação da API é:

https://developer.spotify.com/web-api/endpoint-reference/

## Requisitos adicionais

Como nós somos uma das maiores instituições financeiras independentes da America latina temos que pensar em performance, escalabilidade e testes, segue alguns requisitos adicionais que seria legal ter na sua aplicação:

- Quando o usuário fizer uma requisição seria legal salvar dentro do *redux*, caso ele digite e busque novamente o album nós pegamos uma cópia de lá para não fazer múltiplas requisições para a API.
- Quando o usuário entrar na aplicação podemos exibir uma lista com os últimos albums buscados/clicados para melhorar a experiência.
- Hoje grande parte dos acessos a sites são feitos por celular, um layout responsivo faz todo sentido para nossa aplicação!
- Precisamos ter certeza que nossa aplicação funciona conforme o esperado, alguns testes seriam bem vindos, estamos usando por aqui *enzyme e jest*, mas sinta-se a vontade para testar com o que sente maior conforto.
- Pense que sua aplicação passará por 3 ambientes, DSV - HML - PRD, monte build e use variaveis de ambiente.

# Método de avaliação

- Boas práticas e patterns;
- Código e estrutura da aplicação;
- Componentização e fluxo do dado.
- Facilidade de leitura de código.

Boa sorte e faça o teste da forma que você se sentir confortável.
