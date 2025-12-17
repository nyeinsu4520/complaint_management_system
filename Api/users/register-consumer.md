## POST /api/users/register/consumer

### Functional Requirement: 
FR-01 – Users can register and log in to the system

**Description**
Registers a new customer (end user) in the system using basic personal details.

## Headers

- Content-Type: application/json


### Request Body
```json
{
  "email": "user@example.com",
  "username": "john_doe",
  "phoneNumber": "0123456789",
  "password": "password123",
  "address": "123 Main Street"
}
```

Response:

 - 201 Created – Registration successful

 - 400 Bad Request – Invalid input or user already exists

Notes:

 - Consumers are not assigned a staff role.

 - Consumers can submit complaints and provide feedback.






