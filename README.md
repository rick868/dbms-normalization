# DBMS NORMALIZATION
Normalization is the process of organizing data in a database, to reduce or eliminate <em> data redundancy</em>.

### Why do we need Normalization?
To eliminate unwanted charasteristics like 

1. Insertion anomalies: Insertion anomalies occur when it's not possible to insert data into a dabase because the required fiels are empty or the data is incomplete.

2. Updates anomalies: Update anomalies occur when modifying data in a database and can result in inconsistencies or errors.

3. Deletion anomalies: Deletion anomalies occur when deleting a record from a database and can result in the unintentional loss of data.

### To understand how normalization works, it is important to understand 
1. Keys in databases. That is both the **primary key** and **foreign key**.
2.  Functional dependecy , which helps define the relationships between data in a table.For example, if you know a student’s ID, you can find their name, age, and class. 

#### Features of Database Normalization
<li>
Elimination of Data Redundancy: Data redundancy refers to the repetition of data in different parts of the database. Normalization helps in reducing or eliminating this redundancy, which can improve the efficiency and consistency of the database.</li>
<li>Ensuring Data Consistency:  By eliminating redundancy, normalization helps in preventing inconsistencies and contradictions that can arise.</li>
<li> Improved Database Design: By organizing the data in a structured and systematic way, normalization makes it easier to design and maintain the database.</li>
<li> Avoiding Update Anomalies: Normalization ensures that each table contains only one type of data and that the relationships between the tables are clearly defined, which helps in avoiding such anomalies.</li>


# NORMAL FORMS
**Normal Forms** are different stages of normalization, and each stage imposes certain rules to improve the structure and performance of a database.

### Types of Normal Forms
### 1. First Normal Form (1NF): Eliminating Duplicate Records
  A relation is in first normal form if every attribute in that relation is <b>single-valued attribute</b>. 
  A table is in 1NF if it satisfies the following conditions:
  <li>All columns contain atomic values (i.e., indivisible values).</li>
  <li>Each row is unique (i.e., no duplicate rows).</li>
  <li>Each column has a unique name.</li>
  <li>The order in which data is stored does not matter.</li>

### 2. Second Normal Form (2NF): Eliminating Partial Dependency
  A relation that is in First Normal Form and every non-primary-key attribute is fully functionally dependent on the primary key, then the relation is in <b>Second Normal Form (2NF)</b>.
  A relation is in 2NF if it satisfies the conditions of 1NF and additionally. **No partial dependency** exists, meaning every **non-prime attribute (non-key attribute)** must depend on the **entire primary key**, not just a part of it.

###  3. Third Normal Form (3NF): Eliminating Transitive Dependency
  A relation is in 3NF if it satisfies 2NF and additionally, there are **no transitive dependencies**. In simpler terms, **non-prime attributes** should not depend on other **non-prime**attributes.
  
### 4. Boyce-Codd Normal Form (BCNF): The Strongest Form of 3NF
  BCNF is a stricter version of 3NF where for every **non-trivial functional dependency** (X → Y), X must be a superkey (a unique identifier for a record in the table).  

### 5. Fourth Normal Form (4NF): Removing Multi-Valued Dependencies
  A table is in 4NF if it is in BCNF and has no **multi-valued dependencies**. A **multi-valued dependency** occurs when one attribute determines another, and both attributes are independent of all other attributes in the table.

### 6. Fifth Normal Form (5NF): Eliminating Join Dependency
  5NF is achieved when a table is in 4NF and all join dependencies are removed. This form ensures that every table is fully decomposed into smaller tables that are logically connected without losing information.

### Advantages of Normal Form
1. Reduced data redundancy
2. Improved data consistency
3. 
