
# User Auth Manager API

This is an User Authentication Manager API made using NEXT.js and Typescript.


## Features

- Auth Register
- Auth Login
- Find All Users
- Update User
- Delete User


## Documentation

[Local Swagger Doc](http://localhost:8080/api-docs)

## Postman Collection

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://app.getpostman.com/run-collection/10352918-7a7d3681-8a61-49c0-904e-52c1b698b9b8?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D10352918-7a7d3681-8a61-49c0-904e-52c1b698b9b8%26entityType%3Dcollection%26workspaceId%3De5a5314a-c857-4e38-8a96-1a274751454a)

## Run Locally

Clone the project

```bash
  git clone https://github.com/victorrosbar/user-auth-api.git
```

Go to the project directory

```bash
  cd user-auth-api
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


## API Reference

#### Register user

```http
  POST /auth/register
```

```json
{
    "email": "jondoe@email.com",
    "password": "Pwd&6767",
    "username": "JonDoe12"
}
```
| Description |
| :- |
| Validation pattern is applied for email, username and password|

#### Login

```http
  POST /auth/login
```

```json
{
    "email": "jondoe@email.com",
    "password": "Pwd&6767"
}
```

#### Get All Users

```http
  GET /users
```

| Description |
| :- |
| **Required**: Be logged in with the one user to get the cookie token |

#### Update User

```http
  PATCH /users/${id}
```

| Description |
| :- |
| **Required**: Be logged in with the respective user to get the cookie token |

#### Delete User

```http
  DELETE /users/${id}
```

| Description |
| :- |
| **Required**: Be logged in with the respective user to get the cookie token |

