# Systematically Approaching Design Stages

### Intro

:heavy\_check\_mark:A database and an application together provide a comprehensive <mark style="color:orange;">**picture of a real-world system**</mark>**.**

:heavy\_check\_mark:Data modeling is a <mark style="color:orange;">**structure design process**</mark>.

:heavy\_check\_mark:You explore your choices by using analysis, abstraction, experience, heuristics, and creativity

:heavy\_check\_mark:Developing a data model is an <mark style="color:orange;">**iterative process:**</mark> you develop a model, check it with domain experts, and refine the model.

:heavy\_check\_mark:It can serve as an effective <mark style="color:orange;">**communication tool**</mark> between domain experts and developers.

### Relational Data Model

Represents data in the form of two-dimensional tables consisting of rows and columns. Each table represents a real-world entity (person, place, thing, or event) about which you collect information.

#### Data-modeling phases

* <mark style="color:blue;">**Conceptual phase**</mark> As a database designer, in this phase, you collect all business requirements and rules in cooperation with business domain experts. You can create a conceptual schema by using different methods:
  * object role modeling (ORM) method. An ORM diagram documents a business problem.&#x20;
  * the entity relationship (ER) method. Especially the Integration Definition for Information Modeling (IDEF1X) method
  * Unified Modeling Language (UML), although this language suits application design better than database design.
* <mark style="color:blue;">**Logical phase**</mark> During the logical phase, you represent data that is already grouped logically in entities by adding attributes and relationships between entities. ER diagrams document this relational design. The most-used ER models are the Extended ER model and the IDEF1X model.
* <mark style="color:blue;">**Physical phase**</mark> You implement the relational model physically, in a database on a relational database management system (RDBMS) such as Microsoft SQL Server. No matter which method you use for implementation (automatically via a tool or manually), you have to prepare DDL statements for creating database objects in a language that your RDBMS understands.

In addition to these phases, when you are modeling a database, you can start with another schema, called the <mark style="color:blue;">**external schema**</mark>, that usually comes from the application design process but that can be a good starting point for data modeling. The external schema shows how your system will be used. A common way to show the external schema is by using UML Use Case diagrams. Table 2-1 shows all four stages in a condensed format.

![Table 2-1 Data Modeling Stages](https://learn.microsoft.com/en-us/previous-versions/tn-archive/images/cc505843.table\_c02623422\_1\(en-us,technet.10\).png)

