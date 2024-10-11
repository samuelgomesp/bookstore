# Bookstore

Projeto criado com intuito de simular um programa que cria produtos e ordens de compra com a utilização de classes em JavaScript, nesse caso estamos criando livros e posters. São usadas funções construtoras para os produtos e também foram desenvolvidas funções para criar ordens, salvar usuários e armazenar dados dos pedidos.

## Tecnologias utilizadas 

<div align="center"> 
<img align="left" alt="Node" height="30" width="30" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg">
<img align="left" alt="Javascript" height="30" width="30" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg">

</div>
<br/><br/>

## Exemplo de Uso

```javascript
//Aqui ficam todas as entities e as funções
const App = require('./App')

const app = new App()

app.createAuthor('J. R. R. Tolkien', 'British', '...')

const authors = app.getAuthors()

app.createBook('O Hobbit', '...', 'fantasy', 300, authors[0], '...', 19.99, 100)

const books = app.getBooks()

app.createUser('Samuel', 'samuel@email.com', '123456')

const users = app.getUsers()

app.showDatabase()

const items = [
  {
    product: books[0],
    quantity: 2
  },
  {
    product: books[1],
    quantity: 1
  },
  {
    product: books[3],
    quantity: 1
  }
]

app.createOrder(items, users[0])

app.showDatabase()
```
