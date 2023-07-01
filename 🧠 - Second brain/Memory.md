 Related topics: [[Hardware]], [[Computer Science]]

The memory is the physic element of the computer in which we store all the zeros and ones which represent our information, indeed they're a bunch of spaces where we can store values, let's abstract that idea and use it as a sort of "canvas" where each cell in the grid is a byte: 

![[Memory methapor.png]]

Every time we create a [[Variables|variable]] we're taking or more cells of that grid, (depending on the [[Data type]]).

Now to identify each cell or space of this grid we just enumerate them, but using [[Hexadecimal]] system: 

![[Addresses of memory in hexadecimal.png]]

Now it turns out that there can emerge some ambiguities, confusions, 10 can be ten in decimal system but is also sixteen in [[Hexadecimal]], so to avoid these confusions we prefix them, to know certainly that we're dealing with [[Hexadecimal]] system. 

![[Addresses of memory with prefixes.png]]

# Garbage values

When we're dealing with memory, reserving and freeing spaces, it of course happens all time that we reuse memory before used for other sakes, and sometime we can find what's call a garbage value, that is a value or information which had a use in other context, but know they don't make sense for us. And that's why is important to initialize memory once we ask for it.


# Memory distribution 

Let's understand how the memory distributes all the things which it has to save.

## Machine code

when you click on a program of course the first thing which is put on the very top of the memory is the machine code, like the compiled code of your program, therefore is easily accessible for the computer on run time. 

## Globals

Right on bottom of the machine code the globals are saved, which are just those variables of global scope which you store or declare out of the main function.

## Heap and stack

Is a big chunk of remnant memory where we store all those locations which are changing throughout the execution of the code, as the local variables, what we reserve with malloc and free with free. 

The difference between heap and stack is that, heap is the memory used for the principal code and it starts to use space from top to bottom, whilst stack is where functions have variables and arguments store temporally, and it grows in opposite direction, starts using the bottom of the memory and grows toward the top of it. 

![[Memory distribution.png]]

Now we can notice new errors which we can get, and it turns out that if we start to ask form memory and memory and memory either with the heap, stack or even both, it can happen that we access to memory which is being for the other, this errors are called overflows: 

+ Heap overflow // When the heap tries to access to memory which is being used for the stack
+ Stack overflow // When the stack tries to access to memory which is being used for the heap 

This both errors are just incarnations of what we call buffer overflows, a buffer is just a chunk of memory of the computer which is being used with a specific purpose. 

Other difference between the heap and stack is that meanwhile stack is static memory and is defined once we compile de code, heap is dynamic and is what vary through the code execution. 

The heap memory has to be managed manually, while the stack is mostly managed by the complier. 