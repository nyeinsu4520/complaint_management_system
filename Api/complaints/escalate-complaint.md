## POST /api/complaints/{id}/escalate

**Functional Requirement**  
FR-04 – Help desk / support staff can assign, escalate, and resolve complaints

**Description**  
Escalates a complaint to support staff.

**Headers**
- Content-Type: application/json

**Request Body**
```json
{
  "reason": "Requires technical investigation"
}
```

Response

 - 200 OK – Complaint escalated successfully