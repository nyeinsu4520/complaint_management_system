## GET /api/complaints/company/{companyId}

**Functional Requirement**  
FR-05 (Partial / Design-level) – Complaints can be managed per company

**Description**  
Retrieves all complaints related to a specific company.

**Headers**
- Content-Type: application/json

**Response**
- 200 OK – List of company complaints returned

**Notes**
- Used by help desk and support staff
- Demonstrates multi-tenant data separation
