# Structure of Relational Databases
	Attributes -> Colums 
		Domain -> Set of allowed values of a column 
		values are required to be atomic (indivisible)(generally)
		null is member of all domains indicating value -> "Unknown"
	Tuples -> Rows 
	Relations are Unordered
#  Database Schema
	DB S -> logical structure of DB 
	DB Instance -> snapshot of the Data in the DB given instant in time 
	
	![[Pasted image 20240830113551.png]]
#  Keys
Why
	![[Pasted image 20240830140902.png]]
	Why to "Uniquely identifying the Tuples"
Super Key 
	set of attributes to uniquely identify a tuple 
	![[Pasted image 20240830141319.png]]
Candidate Key 
	minimal super keys is called a candidate key 
	![[Pasted image 20240830141439.png]]
Primary key 
	unique and not null 
	chosen from candidate key 
	chosen by DBA
	![[Pasted image 20240830141739.png]]
Alternate Key 
	![[Pasted image 20240830141823.png]]
Unique Key 
	![[Pasted image 20240830141908.png]]
	
Composite key -> key out of more than one attribute 

Foreign key 
	deals with 2 tables 
	![[Pasted image 20240830142046.png]]
	

#  Schema Diagrams
	![[Pasted image 20240830142249.png]]


# Relational Query Languages
	Relational Algebra 
	
		[[Relational algebra]] -> Separate Page given 


