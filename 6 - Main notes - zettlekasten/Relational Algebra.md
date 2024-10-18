Date: 2024-10-15     Time: 21:04

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby

Tags : [[Computer Science]] ,  [[DBMS]]  

# Relational Algebra

- Relational algebra that is used in database theory that uses algebraic structures for modelling data and queries on it with well founded semantics.
- Main application - Theorotical foundation for relational databases and query languages(sql) for these databases . 
- ***Main purpose***: To define operators that transform one or more input relation into an output relation. These relations can be combined to create complex queries 

Key operations in Relational Algebra:

• **Selection (σ)**: Extracts rows from a relation based on a given condition.

• **Projection (π)**: Selects specific columns from a relation.

• **Union (∪)**: Combines the results of two relations, removing duplicates.

• **Set Difference (−)**: Returns tuples from one relation that are not in another.

• **Cartesian Product (×)**: Combines all tuples from two relations.

• **Join (⋈)**: Combines related tuples from two relations based on a common attribute.


  

Relational Algebra forms the theoretical foundation for SQL and is crucial for query optimization in relational databases.

---
### Why all this? - the question i asked myself
Languages like SQL are **declarative**, meaning you specify **what** you want, not **how** to get it. The DBMS optimizes the query and finds the best way to retrieve the data, which is far more efficient than manually coding data access logic into software.

• Without a query language, developers would need to write complex loops and conditions to filter and retrieve data, leading to more error-prone, less readable code.

Extracting relevant data. Use query languages to retrieve specific data from a large database quickly, avoiding manual extraction.

---

# References
Similar notes and source ideas
[Wikipedia link](https://en.wikipedia.org/wiki/Relational_algebra)



