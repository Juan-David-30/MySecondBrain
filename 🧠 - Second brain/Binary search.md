---
Alias: Search
---

Unlike the [[Linear search]] the binary search requires the data set to be arranged or sorted, but it has the advantage of being widely faster and efficient as the problem gets larger. 

Binary search in pseudocode is: 

+ Repeat until the subarray is of size < 1:
	+ Calculate the middle point fo the current array.
	+ If the target is at the middle, stop. 
	+ Other wise, if the target is less than that middle, repeat changing cutting the array to be just the left half. 
	+  Other wise, if the target is greater than that middle, repeat changing cutting the array to be just the right half. 


![[Binary search.png]]

it has the following performance: 

O(log n)
$\Omega$(1)

```ad-info

title: Remember


When you're thinking in the performance of 
```
