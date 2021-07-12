# snake-game-js
Clássico jogo da cobrinha (bem simples) em JavaScript.
<img src="sprite-snake.jpg" alt="drawing" width="50"/>


## Rodando localmente 1 (apenas para alunos usando o computador)
Você pode rodar o jogo abrindo o arquivo [_views/pages/jogo.html_](views/pages/jogo.html) com o seu navegador.

```sh
$ git clone https://github.com/ifal-riolargo/snake-game-js.git # clone a aplicação para sua máquina local (ou faça antes um fork e clone do seu próprio repositório)
$ cd snake-game-js
$ firefox views/pages/jogo.html # ou use outro navegador ex. google-chrome 
```

----

## Rodando localmente 2
O jogo usa a infraestrutura do Node.js para publicação no Heroku. Por este motivo, você pode rodar um servidor localmente e executar o jogo.

Antes, você precisa ter o [Node.js](http://nodejs.org/) e o [NPM](https://www.npmjs.com/) instalados.
<br><br>
Para quem for usar o Termux, instale com o comando abaixo.
```sh 
$ pkg install nodejs
```

Para quem usa Ubuntu, use os comandos abaixo.
```sh 
$ sudo apt update
$ sudo apt install nodejs
$ sudo apt install npm
```
<br>
Agora execute.

```sh
$ node --version # verificar versão do node
$ npm --version # verificar versão do NPM
$ git --version # verificar versão do GIT
$ git clone https://github.com/heroku/node-js-getting-started.git #só execute clone novamente, se vc ainda não fez clone do projeto
$ cd node-js-getting-started
$ npm install
$ npm start
```

Pronto. Sua aplicação deve executar em [localhost:5000](http://localhost:5000/).

----

## Deploying no Heroku
###### Obs. Heroku CLI não possui versão oficial para o Termux

Agora você pode fazer deploy da suaplicação no Heroku.
Antes, você precisa ter o Heroku CLI que vai ajudar a gerenciar e dimensionar seus aplicativos, provisionar complementos, visualizar seus logs de aplicativo e executar seu aplicativo localmente. 

```sh
$ sudo snap install heroku --classic 
```



```sh
$ heroku login # isso deve abrir o navegador e pedir para você entrar com seu login e senha no Heroku
$ heroku create #cria um repo remoto em heroku.com e aponta o seu repo local para lá 
$ git push heroku main #envia sua aplicação para o heroku
$ heroku open #abre o navegador na sua aplicação, executando em um servidor na nuvem
```

Pronto. Você verá sua aplicação executando em um servidor na nuvem. Basta copiar o link do navegador e você poderá mostrar sua aplicação para seus amigos.

<!-- or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy) -->

----

## Importante

Para mais informações sobre como usar Node.js no Heroku, veja a documentação oficial (em inglês):

- [Getting Started on Heroku with Node.js](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Best Practices for Node.js Development](https://devcenter.heroku.com/articles/node-best-practices)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)
