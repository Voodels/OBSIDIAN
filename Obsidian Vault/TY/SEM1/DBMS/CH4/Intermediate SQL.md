**Joins** 

**Trigger**

**ER Model**
	Design Phase 
		initial 
		second 
		final phase 
	ER -> 
		entity -> object that exists and is distinguishable from other objects 
		entity set -> set of entities of same type and same properties 
		![[Pasted image 20240830210426.png]]
		
**PrevTopics**

**Normalization**

	Designing a database in such a way that the redundancy are minimised as well as anomalies 
    redundancy -> same values repeated over and over again 
	effectively desiging a DB 
	
## Levels of NF 
		1NF
			1.Every column/attribute need to have a single value 
			2.Each row should be unique. Either throught a single or multiple colums.Not Mandatory to have a primary Key 
		2NF
			1.Must be in 1NF 
			2.All non key attributes must be fully dependent on candidate key 
			if non-key column is partially dependent on candidate key(subsets of colums forming candidate key) then split them into seperate tables 
			3.Every table should have primary key and relationship between the tables should be formed using foreing key 
			
			![[Pasted image 20240830212241.png]]
			

**SQLvsNOSQL**

**Query Parsing**
![[Pasted image 20240830194239.png]]
