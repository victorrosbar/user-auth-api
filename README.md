
# User Auth Manager API

This is an User Authentication Manager API made using NEXT.js and Typescript.


## Features

- Auth Register
- Auth Login
- Find All Users
- Update User
- Delete User


## Documentation

[Swagger Doc](http://localhost:8080/api-docs)


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
    "password": "password",
    "username": "JonDoe"
}
```

#### Login

```http
  POST /auth/login
```

```json
{
    "email": "jondoe@email.com",
    "password": "password"
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

