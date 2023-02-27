> **problem statement**
we have  created a db usig the command 
```
create database dbname;
create database library;
```

once the db is **created** crete a table loans
```
create database tablename;
CREATE TABLE loans(
Id Integer, 	
FirstName	Text,
LastName	Text,
Email	Text,
LoanAmount	Integer,
Purpose	Text,
Status Text);
```

let us __insert__ the values into the table
```
INSERT INTO loans(
 Id,
 FirstName, 
 LastName, Email, 
 LoanAmount, 
 Purpose, 
 Status) 

VALUES(
 0,
"firstname",
"lastname",
"email",
 0,
"purpose",
"status");
```

let us **read** all the values in this table use __select__
```
select * from loans;
```

let us read the values basing on _**condition**_ use **where**

```
SELECT * from loans where Status = "approved";

SELECT * from loans where LoanAmount > 1;
```
let us find **average**
```
SELECT AVG(LoanAmount) FROM loans;
```

let us __update__ status from approved to pre-approved
```
UPDATE loans SET Status = "pre approved" where Status = "approved";
```

let us  __delete__ record basing on name
```
DELETE FROM loans WHERE FirstName = "name";
```