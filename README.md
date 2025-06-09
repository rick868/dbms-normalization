# DBMS NORMALIZATION
Normalization is the process of organizing data in a database, to reduce or eliminate <em> data redundancy</em>.

### Why do we need Normalization?
To eliminate unwanted charasteristics like 

1. Insertion anomalies: Insertion anomalies occur when it's not possible to insert data into a dabase because the required fiels are empty or the data is incomplete.

2. Updates anomalies: Update anomalies occur when modifying data in a database and can result in inconsistencies or errors.

3. Deletion anomalies: Deletion anomalies occur when deleting a record from a database and can result in the unintentional loss of data.

### To understand how normalization works, it is important to understand 
1. Keys in databases. That is both the **primary key** and **foreign key**.
2. 
3. Functional dependecy , which helps define the relationships between data in a table.For example, if you know a student’s ID, you can find their name, age, and class. 

#### Features of Database Normalization
<li>
  Elimination of Data Redundancy: Data redundancy refers to the repetition of data in different parts of the database. Normalization helps in reducing or eliminating this redundancy, which can improve the efficiency and consistency of the database.
  
  Ensuring Data Consistency:  By eliminating redundancy, normalization helps in preventing inconsistencies and contradictions that can arise.
  
  Improved Database Design: By organizing the data in a structured and systematic way, normalization makes it easier to design and maintain the database.
  
  Avoiding Update Anomalies: Normalization ensures that each table contains only one type of data and that the relationships between the tables are clearly defined, which helps in avoiding such anomalies.
</li>

# NORMAL FORMS
**Normal Forms** are different stages of normalization, and each stage imposes certain rules to improve the structure and performance of a database.

### Types of Normal Forms

