# cypress.io

Apresentação

https://www.cypress.io/
https://www.cypress.io/blog

Caracteristicas:
 * Ferramenta para teste e2e/integração
 * javascript

videos do criador do cypress:
- https://www.youtube.com/watch?v=5XQOK0v_YRE
- https://www.youtube.com/watch?v=pJ349YntoIs


Requesitos minimos
javascript
como funciona um projeto node(package.json e npm ou yarn)




# criar pasta do projeto

### criando uma pasta para o projeto
```sh
mkdir project-e2e-name
```

### criar package.json
com yarn
```
yarn init -y
```

com npm
```
npm init -y
```


adicionar cypress localmente como depemdencia de desenvolvimento

com yarn
```
yarn add cypress -D
```

com npm
```
npm install cypress --save-dev
```


## abrindo o cypress

diretamente pela linha de comanado
```
./node_modules/.bin/cypress open
```

atraves de um npm script

adicionando um script no package.json
```json
{
  "scripts": {
    "cy:open":"cypress open"
  },
}
```

executando com yarn
```sh
yarn cy:open
```

executando com npm
```sh
npm run cy:open
```


excutando cypress diretamente pelo yarn
```
yarn cypress open
```







