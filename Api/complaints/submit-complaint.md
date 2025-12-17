## POST /api/complaints/register

### Functional Requirement: 
FR-02 – Users can submit complaints linked to a company

**Description**
Allows a logged-in user to submit a complaint associated with a specific company.
The complaint is linked to both the submitting user and the selected company.

## Headers

Content-Type: application/json

### Request Body

```json
{
  "userId": 5,
  "companyId": 1,
  "details": "Unauthorized transaction detected",
  "severity": "HIGH"
}
```

Response

 - 201 Created – Complaint submitted successfully

 - 400 Bad Request – Invalid input or missing required fields

Notes

 - The userId is provided in the request body to identify the user submitting the complaint.

 - In this proof-of-concept, user identity is managed at the application level.

 - Authentication and access control are simplified to keep the scope achievable.