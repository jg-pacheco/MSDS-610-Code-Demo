# MSDS-610-Code-Demo

## Topic: Database Keys

In this assignment we discussed the implementation of database keys and their importance in managing data within a database. Included in this repository are the SQL queries and the data used within the code demo.

### 1. Creating the Tables
The queries in this section create the tables using the provided data and incorporate unique, primary, and foreign keys. The first table is the student table and uses the data in Student.csv. The student table consists of 5 columns with 2 of those columns being unique keys and 1 column being a primary key. The second table is the topic table and uses the data in topic.csv. The topic table consists of 2 columns with 1 column being a foreign key.

### 2. Unique Keys
A unique key establishes a constraint on a column where all data entered in that column must be unique. Thus, there can be no duplicates inserted into that column. In the student table, cell_phone and passport_id were both unique columns. We were able to leave null values in those columns, but could not insert a row into the table that contained a duplicate cell phone number or passport ID. The queries demonstrate the error that is raised when a duplicate is attempted to be inserted into a table's unique key.

### 3. Primary Keys
A primary key is similar to a unique key while also including the additional constraint of not Null. This prevents the data in that column from being a duplicate or being Null. In the student table, student_id was the primary key and it served to identify every student as no two students could have the same student ID and every student had to have a student ID. The queries demonstrate the error that is raised when a Null value is attempted to be inserted into a table's primary key.

### 4. Foreign Keys
A foreign key serves as a reference from a child table to a parent table. It establishes a constraint on a child table's column by preventing data from being inserted into that column if it does not exist in the parent table's column. A foreign key also prevents data from being deleted from the child table's column if it exists in the parent table's column. The queries demonstrate the error that is raised when a value is attempted to be inserted into the child table's foreign key when it does not exist in the parent table's column. The queries also display the error that occurs when a value is attempted to be deleted from the child table's foreign key when it does exist in the parent table's column.
