## POST /api/feedback

**Functional Requirement**  
FR-03 – Users can view and track their complaints

**Description**  
Allows users to submit feedback for a resolved complaint.

**Headers**
- Content-Type: application/json

**Request Body**
```json
{
  "complaintId": 10,
  "rating": 5,
  "comment": "Very satisfied with the resolution"
}
```

Response

 - 201 Created – Feedback submitted successfully