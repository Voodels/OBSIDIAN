## SQL parts 
	DML 
	Integrity -> DDL specifies the Intergrity constrains 
	View -> DDL 
	Transaction Control -> 
	Embedded SQL and Dynamic SQL -> integrating in high level languages 
    Authorization 
## DDL 
	data definition language 
		specifies 
			-> Schema 
			 types of attributes 
			 The integrity constrains 
			set of indices to be maintained 
			Security and Auth for each relation 
			Physical storage structure of each relation on disk 
## Domain 
	types 
		char(n)-> fixed length character string 
		varchar(n)-> varible length char strings with user specifed max length 
		int -> integer 
		small int
		numeric(p,d) -> p digits , d decimal points 
		real,double precision -> floating points 
		 float(n) -> 

## Integrity Constrain
	3 types 
		primary key 
		foreign key reference r 
		not null 
	any update voilating the IC is prevented 

|               |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Create Table  | create table r<br>(A1 D1, A2 D2, ..., A n D n,<br>(integrity-constraint1),<br>...,<br>(integrity-constraintk))                                                      |                                                                                                                                                                                                                                     |
| Insert        |                                                                                                                                                                     | insert into instructor values ('10211', 'Smith', 'Biology', 66000                                                                                                                                                                   |
| Delete        |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| Drop Table    |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| Alter         |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| select clause |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| Where clause  |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| From clause   |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
| Rename        | old-name as new-name                                                                                                                                                | Find the names of all instructors who have a higher salary than<br>some instructor in 'Comp. Sci'.<br>• select distinct T.name<br>from instructor as T, instructor as S<br>where T.salary > S.salary and S.dept_name = 'Comp. Sci.’ |
| Self Join     | join -> cross product + some condition              therefore we make alias of a table ans use the two new with some condition ![[Pasted image 20240830175603.png]] |                                                                                                                                                                                                                                     |
|               |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
|               |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
|               |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
|               |                                                                                                                                                                     |                                                                                                                                                                                                                                     |
