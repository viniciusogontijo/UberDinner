# Buber Dinner API

- [Buber Dinner API](#buber-dinner-api)
  - [Auth](#auth)
    - [Register](#register)
      - [Register Request](#register-request)
      - [Register Response](#register-response)
    - [Login](#login)
      - [Login Request](#login-request)
      - [Login Response](#login-response)

## Auth

### Register

#### Register Request

```js
POST /auth/register
```

```json
{
    "firstName": "João",
    "lastName": "Couve",
    "email": "joaodascouve@gmail.com",
    "password": "joao123!"
}
```

#### Register Response

```js
200 OK
```

```json
{
  "id": "d89c2d9a-eb3e-4075-95ff-b920b55aa104",
  "firstName": "João",
  "lastName": "Couve",
  "email": "joaodascouve@gmail.com",
  "token": "eyJhb..z9dqcnXoY"
}
```

### Login

#### Login Request

```js
POST /auth/login
```

```json
{
    "email": "joaodascouve@gmail.com",
    "password": "joao123!"
}
```

```js
200 OK
```

#### Login Response

```json
{
  "id": "d89c2d9a-eb3e-4075-95ff-b920b55aa104",
  "firstName": "João",
  "lastName": "Couve",
  "email": "joaodascouve@gmail.com",
  "token": "eyJhb..hbbQ"
}
```