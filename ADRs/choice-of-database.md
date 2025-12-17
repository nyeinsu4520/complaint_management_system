## Choice of Database (ADR)

**Context and Problem Statement**

The Complaint Management System (CMS) stores structured data including users, companies, complaints, complaint statuses, and feedback. The database must support relational data, enforce data integrity, and allow efficient querying by user, company, and complaint status. As this system is developed as a proof-of-concept, the database should also be easy to configure, maintain, and integrate with the backend.

**Decision Drivers**

Data Integrity: Strong support for relationships and constraints

Query Flexibility: Efficient querying for complaint tracking and reporting

Reliability: Stable and widely supported technology

Ease of Development: Simple setup with good tooling support

### Considered Options

 - Relational Database (MySQL / PostgreSQL)

 - NoSQL Database (MongoDB)

 - In-Memory Database (H2)

### Decision Outcome

A relational database (MySQL) was selected. The system relies on clearly defined relationships between entities such as users, companies, complaints, and feedback, which are naturally modelled using relational tables. MySQL provides strong data consistency, referential integrity through foreign keys, and reliable query performance. Its ease of setup and widespread support make it well suited for both the proof-of-concept and potential future extension.

**Consequences**

**Positive**

 - Strong data consistency and integrity

 - Clear modelling of relationships using foreign keys

 - Mature tooling and widespread community support

**Negative**

 - Schema changes require database migrations

 - Less flexible than schema-less NoSQL solutions

**Summary of Other Options**

MongoDB: Offers flexible schemas but provides weaker support for complex relational constraints required by the system.

H2: Useful for lightweight testing but not suitable for realistic, persistent data storage.