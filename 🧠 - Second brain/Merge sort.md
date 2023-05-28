---
Topic: sorting
---

Merge sort is one of the fastest [[sorting]] [[algorithms]], but also one of which needs more [[memory]], and that's mainly because it use [[recursion]] to split a data set as much as possible until we got one element and base on it start arranging the elements based in the order, let's understand it better with the [[pseudocode]]: 

+ If the data set's length is equal or less than 1, then return (base case)
+ sort the left half on the data set ([[recursion]])
+ sort the right half on the data set ([[recursion]])
+ Merge the two halves together (sorting them)

We have create a function to merge the halves in a ordered way, the advantage is that we don't have to run on them multiple times because they're sorted, so we just go forwards. 

![[Merge sort.png]]

The performance of this array in the big-O is way better than the [[Select sort]] and [[Bubble sort]]: 

O(n log n)
$\Omega$(n log n)

Then $\Theta$ (n log n)

```ad-info

Notice that the $\Omega$ of this algorithm is lower than the $\Omega$ of [[Bubble sort]]. 

```
