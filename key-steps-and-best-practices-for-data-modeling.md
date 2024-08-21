# Key Steps and Best Practices for Data Modeling

### Intro

The first step in developing a data model is **identifying requirements**. You must communicate with domain experts, key stakeholders, and even end users to gather all the information you need. You can help yourself by using UML Use Case diagrams, if they already exist, and existing reports. You can then **create a conceptual model**, which documents all business requirements and rules as facts. From the conceptual model, you create a logical model. **Alternatively, you can create a logical model directly,** without the conceptual model. In either case, check the conceptual or logical model with domain experts and refine it as needed. Iterate through the model at least a couple of times.

From the logical model, you **create a physical model**. The design process is not finished here, though. Next, you refine the physical model according to security, performance, auditing, availability, and scalability needs. Finally, you build a prototype to test the database design.

### Best Practices

1. **Be especially careful with the scope of the project.** Many projects fail because the scope is not well defined. Alternatively, many developers use scope expansion as an excuse for their bad work. Your customers simply cannot know everything they need in advance. Even if they did know everything they needed today, you have to consider that business changes quickly. Therefore, you must be prepared for several iterations during the design process. Three iterations in refining the model is normal; more iterations than that usually means the scope was not well defined, or the customer requested features that should be part of a different project.
2. **Choose the appropriate methodology.** ER diagrams are an informal standard for the database part of documenting a project, so the ER method should be one of your selected methodologies. In addition, ORM, which is more expressive than the ER model, is useful for presenting complex rules.
3. **Use a professional database-modeling tool.** Tools such as Visio for Enterprise Architects enable forward engineering—creating a logical model from a conceptual model and then creating a physical model from the logical model. Make sure you are familiar with the tool before you start your design.
4. **Include your physical model, the DDL scripts, in a source control system.** You can use Visual Studio Team System for source control.
5. **Start with a strict relational model, but be prepared to make some compromises to satisfy business needs.** For example, usually you have to denormalize some data to achieve satisfactory performance. Document such compromises thoroughly.
6. **Use free models as a starting point.** You can find free models in books and on the Web. Check existing models if you upgrade an application. An upgraded application must provide all the features of the old application; otherwise, users will not be satisfied.
