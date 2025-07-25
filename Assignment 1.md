S##### Assignment 1 

Ankit Yadav ankitmuo@mail.com

##### Git Assignment





**git-clone** = used to bring or clone the repository to the local system which is hosted on GitHub.



**git-add** = used to track your file in git.



**git-commit** = save file in git.



**git-push** = upload git commit to a remote repository on GitHub.



**git-status** = used to know the current status of working tree.



**git-stash** = used to save the uncommitted changes in a git repository.



**git-branch** = used to manage branches which allow user to work on different branches without 

affecting the main branch 



##### MySQL Assignment.



**levels of isolation ?**



**There are four main levels of isolation in database.**

**1. Read Uncommitted**



**Lowest isolation level.**



Transactions can read data modified by other transactions even if those changes are not yet committed .





**2. Read Committed**



A transaction only sees committed changes from other transactions (no dirty reads).



However, non-repeatable reads (data changes between reads in the same transaction) and phantom reads (new rows appearing in repeated queries) can still happen.



**3. Repeatable Read**



Ensures that data read once by a transaction cannot change during that transaction (no dirty reads and no non-repeatable reads).



However, phantom reads are still possible (new rows matching a query could appear if another transaction inserts them).



**4. Serializable**



Highest isolation level.



Transactions are completely isolated, as if run one after another (serially).



Prevents dirty reads, non-repeatable reads, and phantom reads—giving the most consistency but with more performance overhead



**3nf?**

To achieve 3nf the table has to be in 1nf 

which states that every attribute should have atomic(only one value )value.



And then it should be in 2nf for which it has to be in 1nf and no partial dependency should 

be there on primary key 



Then to be on 3nf it has to be in 2nf and there should be no transitive dependency on primary key



**DDL and DML?**

DDl stands for data definition language which mean it is used to create structure of database/table example create ,alter, drop.



where as DML is a data manipulation language it manages data within the schema with command 

like select , insert, update , modify, delete.









**drop truncate delete?**



**DELETE**

**Removes specific rows (records) from a table.**

**The table and its structure stay the same.**

**You can usually undo (rollback) DELETE if you’re inside a transaction.**

**TRUNCATE**

**Quickly removes (deletes) all rows from a table.**

**The table and its structure remain.**

**Usually, you can't undo TRUNCATE.**

**DROP**

**Deletes the entire table from the database, including all its data and structure.**

**The table is gone completely.**

**You can’t undo DROP .**















