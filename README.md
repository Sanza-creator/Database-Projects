# Database Systems Projects

Two projects covering the full database design lifecycle — conceptual modelling through to implementation across relational, document, and graph paradigms.

---

## 1. Database Design & Normalization — Eduvos Exam Management System

### Scenario
Designed a relational database for an institution's exam management process, covering students, parents, specializations, subjects, and exam administrators across multiple departments and campuses.

### What I did
- Performed entity/attribute analysis from a written business scenario and identified primary/foreign keys
- Drew an initial conceptual ERD (crow's foot notation), identifying unresolved many-to-many relationships
- Resolved many-to-many relationships into a final ERD and documented relationship types (1:1, 1:M, M:M) between every entity pair
- Carried out full normalization up to Third Normal Form (3NF)
- Designed a second relational scenario (Online Book database — books, publishers, authors, reviews) including a logical schema diagram and an equivalent graph-database model of the same data
- Wrote relational algebra queries for real business questions (e.g. retrieving publishers by location, filtering books by category and page count, joining authors to their books)
- Modelled database transactions and schedules, and proposed a deadlock-resolution strategy

### Skills demonstrated
`ERD design (crow's foot)` · `Normalization (1NF–3NF)` · `Relational algebra` · `Transaction scheduling & concurrency control` · `Conceptual → logical → graph modelling`

---

## 2. Multi-Database Implementation — Eduvos Enrolment & Online Library Systems

### Scenario
Implemented the same class of enterprise data problem (an enrolment system, and an online library management system) across three different database technologies to compare relational, document, and graph approaches to the same domain.

### What I did
- **Oracle DBMS:** Built a relational enrolment system (departments, instructors, modules, students, registrations) — created tables and sequences, inserted records via parameterised sequences, built a joined view of instructors and their modules, and wrote a stored procedure to register a student for a module while preventing duplicate registrations
- **MongoDB:** Modelled an online library system (books, authors, members, borrowed-books) as five collections, populated them with sample data, and wrote queries to filter books by publication year, calculate total fines collected, delete resolved fine records, and join borrower/book/loan details into a single result set
- **Neo4j:** Modelled the same library system as a property graph — member, author, and book nodes connected via `IS_WRITTEN_BY` and `BORROWED` relationships — then wrote Cypher queries to count an author's books, list all members with their borrowed titles and due/return dates, and identify overdue (unreturned) books

### Why this project
Building the same real-world problem three different ways made the trade-offs between relational, document, and graph databases concrete — for example, how naturally the library's borrowing relationships map onto a graph model versus a relational join.

### Skills demonstrated
`SQL (Oracle)` · `Stored procedures & sequences` · `MongoDB (CRUD, aggregation)` · `Neo4j & Cypher` · `Data modelling across paradigms`

