# Data Models and Query Languages

* **Data models**  most important part of developing software,because
   how we think about the problem that we are solving.
   

  * Most applications are built by layering one data model on top of another :- 
  layer1 ,layer2,layer3,layer4
  
  * layer1:-people , order , actions 
  * layer2:-DataStructure && objects && Api
  * layer3:- Json && XML &&relational &&graph os data
  * layer4:- represent bytes in terms of electrical currents

  # Relational Model && Document Model
  
  * **The relational** model is a way of organizing data in tables or relations
  * **SQL** is used to manage and manipulate data stored in relational databases
  *  **SQL** is supports transaction processing and business data processing
  * The goal of the relational model
was to hide that implementation detail behind a cleaner interface

# NoSQL
* Why NoSql ??

-->need for greater scalability than relational databases

-->widespread preference for free and open source

-->Specialized query operations that are not well supported by the relational model

-->dynamic and expressive data model

* Note-->Different applications have different requirements

* The JSON representation has better locality than the multi-table schema
 * document model is better suited for applications that require more flexible and dynamic data structures
 *  the relational model is better suited for applications that require complex data querying and analysis, and where data consistency and integrity are critical
# Many-to-One && Many-to-Many Relationships



# The network model
* The CODASYL model was a generalization of the hierarchical model
* In the tree
structure of the hierarchical model, every record has exactly one parent; in the net‐
work model, a record could have multiple parents
* The links between records in the network model were not foreign keys, but more like
pointers
* only way
of accessing a record was to follow a  access path.
* access path:- predefined sequence of steps that the database system uses to locate a specific record or set of records

* an access path could be like the traversal of a linked list: start at
the head of the list, and look at one record at a time until you find the one you want

# The relational model
* The relational model laid out all the data in the open and represented it as a collection of tuples or rows.
* In a relational database, the **query optimizer** automatically decides which parts of the
query to execute in which order, and which indexes to use.
 * Query optimizer used by database management systems (DBMS) to optimize and improve the performance of database queries.

 * By optimizing queries, query optimizers can significantly improve the performance of the database system and reduce the amount of time it takes to retrieve and process data

 * in m to m  Doc Models is better because it locality
 * document model can provide better locality than a relational model.
