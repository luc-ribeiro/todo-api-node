<h1 align="center">
Node.ts To do list API
</h1>
<br>

<div align="right">
  Clique <a href="https://github.com/luc-ribeiro/todo-api-node/blob/master/README-PTBR.md">aqui</a> para ver a versão em Português.
</div>

## 💻 Projeto
O projeto consiste em uma API REST para cadastro, leitura, alteração e deleção de "To dos".

## 🚀 Tecnologias

- **Node.js** 
- **Express**
- **TypeScript**
- **PostgreSQL**
- **Sequelize**

### 🔖 Preview

![preview](https://github.com/luc-ribeiro/nodets-todo-api/blob/master/design/preview.gif)

#### Tabela do Banco de Dados

![banner](https://github.com/luc-ribeiro/nodets-todo-api/blob/master/design/bd-preview.png)

<br>

## :page_facing_up: Como utilizar

Faça um clone deste repositório:

```sh
  $ git clone https://github.com/luc-ribeiro/nodets-todo-api.git
```

Instale as dependências:

```sh
  # com npm
  $ npm install

  # com yarn
  $ yarn install
```

Criar um arquivo `.env` na raiz do projeto <br><br>
Nesse arquivo, definir as seguintes configurações:

```sh
PORT=NúmeroDaPortaQueAAplicaçãoIráRodar

PG_DB=NomeDoBancoDeDados
PG_USER=NomeDoUsuárioDoBancoDeDados
PG_PASSWORD=SenhaDoUsuário
PG_PORT=NúmeroDaPortaDoBancoDeDados
```

Criar uma tabela no Banco de Dados com o nome `todos`

Execute o comando:

```sh
  # com npm
  $ npm run start-dev

  # com yarn
  $ yarn start-dev
```

<br>

### Utilizando as rotas

Após definir o número da porta no arquivo `.env`:

`GET` `localhost:NumeroDaPorta/todo` → Irá lista os To Dos cadastrados no Banco de Dados. <br><br>
`POST` `localhost:NumeroDaPorta/todo` → Irá cadastrar um To Do, é necessário informar no Body da requisição o `title`, que será o nome do To Do.<br><br>
`PUT` `localhost:NumeroDaPorta/todo/:id` → Irá atualizar o To Do com o ID informado. Necessário informar o `title` no Body da requisição. <br><br>
`DELETE` `localhost:NumeroDaPorta/todo/:id` → Irá deletar o To Do com o ID informado. <br><br>
