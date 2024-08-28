	-> partition dp 
	 from strivers lec , this is a advanced topic and the pre requist are 1d,2d,3d ....

Matrix multiplication 
	A x B 
	A(i x j) B(k x l)
	 j == k is compulsory 
	 first row of A multiplies with first column of B
	 ![[Pasted image 20240821225148.png]]
	 cost of multiplying is 5 * 4 * 3 == 60 calculations 

MCM is about how to parenthesis these matrix 
![[Pasted image 20240821225326.png]]
Dynamic Programming solution -> 
	example -> 
		![[Pasted image 20240821225408.png]]
		 M[1,1] = A1 = 0 (nothing getting multiplied)
		 ![[Pasted image 20240821225710.png]]
		 ![[Pasted image 20240821233757.png]]
		 minimum of ( m[1,3]= A1*(A2 * A3) ||  (A1*A2) * A3)  )
		 ![[Pasted image 20240821234225.png]]
		 ![[Pasted image 20240821234501.png]]
	      ![[Pasted image 20240821234628.png]]
	      ![[Pasted image 20240821234741.png]]

Time Complexity 
-> O*n^3
       
![[Pasted image 20240821234937.png]]