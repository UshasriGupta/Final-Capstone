# Database Schema

## Users

| Field | Type |
|-------|------|
| id | String |
| name | String |
| email | String |
| password | String |

## Students

| Field | Type |
|-------|------|
| id | String |
| name | String |
| branch | String |
| year | Number |

# API Endpoints

## Register User

POST /api/register

Request:

```json
{
  "name": "Usha",
  "email": "usha@gmail.com",
  "password": "123456"
}
```

Response:

```json
{
  "message": "User Registered"
}
```

## Login User

POST /api/login

Request:

```json
{
  "email": "usha@gmail.com",
  "password": "123456"
}
```

Response:

```json
{
  "token": "jwt_token_here"
}
```

## Get Students

GET /api/students

## Add Student

POST /api/students