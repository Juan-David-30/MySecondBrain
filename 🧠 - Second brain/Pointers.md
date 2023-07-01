Related topics: [[Computer Science]], [[C]]

In C there are two different operators which allows us to play with the pointes, and the computer's [[Memory]]:

+ & (ampersand, returns the direction in memory of a variable).
+ * (De-reference operator, goes to the direction expressed next to it).

And thanks to them we can define and use the pointers, which aren't anything more but a variable or something that contains the address of a value in memory.

```C

int n = 50; // Variable which contains a number

int *p = &n; // Pointer which contains the address of n

```

n is a variable which contains a integer an p is a pointer, more specifically a variable which contains the address of n, to specify or indicate that p is a pointer we use the "\*", and with the "&" we get the address of n: 

![[Pointers grid.png]]

Often we're not interested in the value or address itself rather what interests us is the fact that we can use one value the value saved in the pointer to access to other value, as if it was actually pointing or redirecting us to the other value (that's where the name comes from). 

![[Pointers abstraction.png]]

# Pointers arithmetic

Now we know that the pointers are addresses in memory which are written or assigned with numbers, and we also know how to access to those values, thanks to that we can do a sort of arithmetic with those values and poke around with the memory addresses, let's see an example:

```c
int numbers[2] = {1,2};

  

printf("%p\n", *numbers);

printf("%p\n", *(numbers + 1));

/*
OUTPUT:
1
2
*/

```

Here we can notice, that a array actually is as the strings just the address of the first element in that data structure so to speak, and with adding or moving around with the other directions we can play with that data structure, and indeed that's what is happening underneath the hood when you're using the square brackets notation (numbers[0]).

# Asking for memory to the OS

C has two functions which allows us to ask for memory and of course also free it:

+ malloc (stands for memory allocation) // Returns the direction in memory of the chunk reserved for us.
+ free // frees the chunk of memory previously reserved for us

```C
#include <stdlib.h> 
// We got to use the library standard library


malloc(/*Number of bytes*/) // Returns direction of the first byte reserved

free(/*Direction you want to free*/)

```

It turns out that if for any reason you asks for too much memory or for whatever reason the computer fails in getting a space for you, then it'll return "NULL" which is different to NUL, NUL is the zero unique character also represented with "\\0". Meanwhile "NULL" is the memory address zero, "0x000000" which for convention is always empty. 
