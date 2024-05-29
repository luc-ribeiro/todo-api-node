<h1 align="center">
To do list API
</h1>
<br>

<div align="right">
  Clique <a href="https://github.com/luc-ribeiro/todo-api-node/blob/master/README-PTBR.md">aqui</a> para ver a versão em Português.
</div>

## 💻 Project
The project consists of a REST API for creating, reading, updating, and deleting "To dos".

## 🚀 Technologies

- **Node.js** 
- **Express**
- **TypeScript**
- **PostgreSQL**
- **Sequelize**

### 🔖 Preview

![preview](https://github.com/luc-ribeiro/nodets-todo-api/blob/master/design/preview.gif)

#### Database Table

![banner](https://github.com/luc-ribeiro/nodets-todo-api/blob/master/design/bd-preview.png)

<br>

## :page_facing_up: How to use

Clone this repository:

```sh
  $ git clone https://github.com/luc-ribeiro/nodets-todo-api.git
```

Install the dependencies:

```sh
  # with npm
  $ npm install

  # with yarn
  $ yarn install
```

Create a `.env` file at the root of the project <br><br>
In this file, define the following settings:

```sh
PORT=PortNumberWhereTheApplicationWillRun

PG_DB=DatabaseName
PG_USER=DatabaseUserName
PG_PASSWORD=UserPassword
PG_PORT=DatabasePortNumber
```

Create a table in the Database named `todos`

Run the command:

```sh
  # with npm
  $ npm run start-dev

  # with yarn
  $ yarn start-dev
```

<br>

### Using the routes

After defining the port number in the `.env` file:

`GET` `localhost:PortNumber/todo` → Lists the To Dos registered in the Database. <br><br>
`POST` `localhost:PortNumber/todo` → Registers a To Do, you need to inform the `title` in the request Body, which will be the name of the To Do.<br><br>
`PUT` `localhost:PortNumber/todo/:id` → Updates the To Do with the informed ID. It is necessary to inform the `title` in the request Body. <br><br>
`DELETE` `localhost:PortNumber/todo/:id` → Deletes the To Do with the informed ID. <br><br>
