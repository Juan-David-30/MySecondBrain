---
Topic: sorting
---

The select sort [[Algorithms|Algorithm]] is a algorithm which sorts a given data set, in pseudocode looks like this: 

+ Repeat until no unsorted elements remain: 
	+ Search the unsorted part of the data to find the smallest value
	+ Swap the smallest found value with the first element of the unsorted part

Every time we iterate on the data set, the first element will be ordered, so we won't have to iterate on it again. 

![[Select sort.png]]

Performance in big-O and $\Omega$ :

O($n^2$)
$\Omega$($n^2$)

so $\Theta$($n^2$)