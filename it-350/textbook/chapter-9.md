## Chapter 9: Transaction Management

### Definitions
- `Transaction` A logial unit of work that contains one or more SQL statements and takes the database from one consistent state to another
- `Compensating transaction` A transaction to undo the effects of a previous transaction

### General Notes
- There are two ways a transaction can terminate
	- It can succeed in which case it is classified as "committed"
	- It can fail and be classified as "aborted"
- Unless the programmer manually delimits the beginning and end of transactions, there's no way for the DBMS to know when things start and stop
	- This usually results in the DBMS treating the entire running program as one transaction
