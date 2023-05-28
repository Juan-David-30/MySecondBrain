---
Topic: Algorithms 
---
Related topics: [[Computer Science]]

Recursion is the ability of a [[Functions|function]] of call itself, so one function can itself:

```C

void row(int length)
{
	if (length > 1)
	{
		row(length - 1); //here is calling itself
	}
	for (int i = 0; i < length; i++)
	{
		printf("#");
	}
	printf("\n");
}

```

The function above calls itself so is regarded as a recursive function.

The recursion allows us to create sometimes sort of loops, but that's not it's main function, it is mainly useful to split a charge into smaller slices so is more manageable. A clear example of it is the [[Merge sort]]. 

So the recursion is mainly used to solve a problem by splitting it into smaller and smaller problems until we can't split it more or we know the answer by a fact, this is called base case. 

![[Factorial recursion algorithm.png]]

The steps are solve from bottom to top, this steps or calls of the function are called call stack. 