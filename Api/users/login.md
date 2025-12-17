## POST /api/users/auth/login

### Functional Requirement
FR-01 – Users can register and log in to the system

**Description**
Authenticates a user using email and password.

## Headers

Content-Type: application/json

### Request Body
```json

{
  "email": "user@example.com",
  "password": "password123"
}
```

Response:

 - Status: 200 OK - Login successful

 - Returns authenticated user details

Notes

 - Role-based access control is applied after authentication.
