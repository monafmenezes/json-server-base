<h1 align="center">
  <img alt="KenzieHub" title="KenzieHub" src="https://kenzie.com.br/images/logoblue.svg" width="100px" />
</h1>

<h1 align="center">
  User - API
</h1>

<p align = "center">
Este é o backend é para atividade JSON-Server: Fake-API do início ao Deploy, que tem como objetivo criar uma API-fake, para criar um frontend de qualidade. 
</p>

O url base da API é https://user-api-kenzie.herokuapp.com/users

<p align="center">
  <a href="#endpoints">Endpoints</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</p>

## **Endpoints**

A API tem o total de 2 endspoints, sendo o principal de usuários (user).

## Rotas que não precisam de autenticação

<h2 align ='center'> Listando usuários </h2>
Para acessar a lista de usuários podemos acessar dessa forma: 
`GET /users -  FORMATO DA RESPOSTA - STATUS 200`

```json
[
    {
    "email": "kenzinho@mail.com",
    "password": "$2a$10$YQiiz0ANVwIgpOjYXPxc0O9H2XeX3m8OoY1xk7OGgxTnOJnsZU7FO",
    "name": "Kenzinho",
    "age": 38,
    "id": 1
    }
]
```
<h2 align ='center'> Listando comentários </h2>
Para acessar a lista de comentários podemos acessar dessa forma, só usuários logados terão acesso a leitura: 
`GET /comments -  FORMATO DA RESPOSTA - STATUS 200`

```json
[
    {
    "userId": 1,
    "comment": "olá"
    }
]
```

