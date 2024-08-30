![[ch1.pdf]]

# Data base applications 
	DBs are used in Enterprises-> 
						for managing 
							sales -> customers, products, purchases
							 accounting -> payments, receipts, assets
							 human resources -> Information about employees, salaries, payroll taxes.
	  manufactoring 
	  banking 
	  university -> grades , registration of courses 

# Purpose of DB 
	 data redundancy and inconsistency => cuz of many different files  
	 difficulty in accessing data 
	 data isolation 
	 integrity problem -> buried in code , hard to change 
	 atomicity of updates 
	
	 concurrent updates 
	 security problems 
	  
# Data models 
	a collection of tools for describing 
		data 
		data relationships 
	    data sematics 
		data constrains 
# Instance and Schema 
	As the types and variables in programing 
	Logical schema
		 overall logical strcuture,ex class of object 
	Physical chema 
		the overall physical structure of db 
	Instance 
		the actual content of DB at a perticular point in time 
# Physical Data Independence 
	the ability to modify the physical schema without changing the logical schema 
	 applications depends on the logical schema 
	  interface -> as in typescript should be well defined so change in componennt 1 using db dosent affects the change in component 2 

# DDL
	Data definition Language 
		notaion for defining the schema 
	DDL compiler generates a set of tabke templates stored in a data dictionary 
		Data Dictonary 
			Schema 
			Integrity constrains 
			authorization 

# DML
	Data manipulation language 
	  used to update delete access the data organised by db model
	  also known as query language 
    two types -> 
	    Pure 
		    used for optimization 
			    Relational Algebra 
			    Tuple relational Calculus 
			    Domain Relation Calculus 
	    Commercial 
		    SQL 
		
		Procedural DML-> 
			specify what data needed and how to get that 
		Declarative DML-> 
			what data needed without telling how to get that data 

# SQL 
	non proceduralm , input -> table/s op -> table/s 
	to compute complex functions SQL is usally embedded in higher level Language 
		language extensions alloe embedding sql 
		Application program interface (ODBC/JDBC) allows SQL queries to be sent to a DB 


# DB Design 
	Logical design 
		deciding schema 
	Physical Design 
		desiging the physical layout of DB
		
# DB engine 
	db system is partitioned into modules each with imp responsiblity 
		storage manager 
			a program module -> 
				interface between low level data and application programs queris 
			interaction with the OS file manger 
			Efficient storage and retrival and updating 
			implements Data structure   
				stores thedb itseld 
				data dictionary 
				 stores meta data 
				indexes -> pointers to data items with perticular value 
				provides fast access
		query processor 
			DDl interpreter -> records definition in data dictonaries 
					Data Dictionary consists of database metadata. It has records about objects in the database.
						Data Dictionary consists of the following information −

						- Name of the tables in the database
						- Constraints of a table i.e. keys, relationships, etc.
						- Columns of the tables that related to each other
						- Owner of the table
						- Last accessed information of the object
						- Last updated information of the object
			DML compiler -> converts the statement into an evaluation plan consising low level onstructions , performs the query optimisation => picks the lowest cost evaluation plan from available alternatives 
			Query Evaluation Engine 
				execute the lowlvl instructions genrated by the DML compiler 
		Query Processing 
		
			![[Pasted image 20240830111018.png]]
			https://www.geeksforgeeks.org/sql-query-processing/
			
		transation management component 
			A transaction is a collection of operations that performs a single
			logical function in a database application
			Transaction-management component ensures that the database
			remains in a consistent (correct) state despite system failures (e.g.,
			power failures and operating system crashes) and transaction
			failures.
			Concurrency-control manager controls the interaction among the
			concurrent transactions, to ensure the consistency of the database.
		

# DB architectures
	Centralized databases
		• One to a few cores, shared memory
	 Client-server,
		• One server machine executes work on behalf of multiple client machines.
	 Parallel databases
		• Many core shared memory
		• Shared disk
		• Shared nothing
	 Distributed databases
		• Geographical distribution
		• Schema/data heterogeneity

	https://www.geeksforgeeks.org/dbms-architecture-2-level-3-level/

# DB Users 
	4 types 
		Naive Users 
		Application Programmers 
		Sophisticated Users 
		Specialized Users 

# DBA
	person with central control over the system 
		Schema definition
		 Storage structure and access-method definition
		 Schema and physical-organization modification
		 Granting of authorization for data access
		 Routine maintenance
		 Periodically backing up the database
		 Ensuring that enough free disk space is available for normal
		operations, and upgrading disk space as required
		 Monitoring jobs running on the database and ensuring that
		performance is not degraded by very expensive tasks submitted by
		some user
	