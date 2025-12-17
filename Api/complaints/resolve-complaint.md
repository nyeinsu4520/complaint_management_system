## POST /api/complaints/{id}/resolve

**Functional Requirement**  
FR-04 – Help desk / support staff can assign, escalate, and resolve complaints

**Description**  
Marks a complaint as resolved.

**Headers**
- Content-Type: application/json

**Request Body**
```json
{
  "resolutionNote": "Issue resolved and customer informed"
}