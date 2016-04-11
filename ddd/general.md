# DDD best practices

*Highly preferred way:*
- Use Repositories:
  - clearly defined responsibility (fetch the Aggregate Root)
  - acts like a collection / storage locations
  - query method and introducing of _Specification Pattern_ pattern
  - Conceptually encapuslates the set of objects.
  - One-way dependancy between domain and data mapping layers

*Not recommended way:*
- Use DAO's: 
  - responsibilities not clearly defined
  - too much coupling to Entity
  - beeing table-centric
  - DAO interface can quickly becomes a ball of mud hard to maintain and test
