# graphql-mongo-workshop
La mayoría de las aplicaciones actuales tienen la necesidad de obtener datos de un servidor donde esos datos se almacenan en una base de datos. GraphQL es un nuevo estándar API que proporciona una alternativa más eficiente, potente y flexible a REST. Permite que un cliente obtenga solo los datos que necesita de un servidor.
GraphQL a menudo se confunde con ser una tecnología de base de datos, pero esta es una idea falsa, GraphQL es un lenguaje de consulta para API, no para bases de datos. En ese sentido, su base de datos agnóstica y efectiva se puede usar en cualquier contexto donde se usa una API.

## Setup

1. Clona el proyecto
2. `npm install`
3. `node index.js`
4. Go to http://localhost:4000/
5. Disfruta tu graphql server

## Ejemplos a usar

### Agregar un usuario

mutation{
  addUser(fullname:"Ibe Ogele",username:"ibesoft",phone_number:"2348102331921",city:"Enugu"){
    id
    fullname
    username
    phone_number
    city
  }
}

### Obtener usuarios

query{
  getUsers{
    id
    fullname
    username
    phone_number
    city
  }
}

### Obtener un usuario por ID
query{
  getUser(id:"user_id"){
    id
    fullname
    username
    phone_number
    city
  }
}
