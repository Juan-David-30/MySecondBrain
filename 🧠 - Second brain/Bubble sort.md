---
Topic: sorting
---

Bubble sort is a algorithms which allow us to sort elements, it works as follows in pseudo code: 

+ Set swap counter to a non-zero value
+ Repeat until the swap counter is 0:
	+ Reseat swap counter to 0
	+ Look at each adjacent pair
		+ if two adjacent elements are not in order, swap them and add one to the swap counter

![[Bubble sort.png]]

A fact of the bubble sort is that in each iteration the las value will be in order, so we can ignore it in next iterations. 

Performance, big-O and $\Omega$:

O($n^2$)
$\Omega$(n)