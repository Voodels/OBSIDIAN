Types
1) 0/1  -> DP
item -> { Weight + Profit } 
bag = 20kg such that maximum profit must be made in that 20kg 

example:->
	![[Pasted image 20240821193150.png]]![[Pasted image 20240821194622.png]]
	
	 finding final answer
	 6<- final res- max go to above , if its the same then go to again further 
	 upwards 6 - 6 - 5 : now take 5 in answer , max is 8 so now 8-5 = 3 , its in
	 its in array so take 3 -> {1,0,0,1}
							 {3,4,6,5} weights -> max is {1,0,0,1}
							 {2,3,1,4} profits -> max is 6 

2)  Fractional Knapsack Problem -> Greedy
		 selecting maximum profit 
		![[Pasted image 20240821223934.png]]
		 selecting minimum weight 
		 ![[Pasted image 20240821224204.png]]
		 selecting ration of profit by weight 
		 ![[Pasted image 20240821224332.png]]
		 
		 
