Related topics: [[Computer Science]], [[How to represent information]]

Truncation is the lose of decimal values (values after the decimal point), like we saw in [[Integer overflow]], the computers has a limit of precision in the representation of information and in this case of numbers, real numbers in this case.

As we may infer we can represent decimal values through the use of the [[Variables]] type float or double for the double of decimal values being float of 32 bits whilst double for 64 bits, the more bits we use the more accurate, for the reasons explained in [[Computers decimal imprecision]].

This lose of decimal values can be generated because of multiple things, like defining a variable with a wrong [[Data type]], for example with integer when we should use either float or double, or even for not casting the values which we're operating, casting is the process of transforming a type of value to other, and for example in [[C]] when we're assigning a the result of a operation to a variable, we have to translate the values which we're operating before operating them, so we get the correct value without truncation: 

```C
#include <stdio.h>

int main(void)
{
	
	int x = 1;
	
	int y = 3;
	
	float result = (float)x/(float)y; //Casting values and saving the result
	
	printf("%f\n", result);
	
}

```


