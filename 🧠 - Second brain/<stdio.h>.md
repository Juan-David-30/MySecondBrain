Related topics: [[C]]

This is the [[C]] header related to the functions about I/O (Input/Output) Inputs and outputs.

# Printing things

## printf

Prints a formatted string: 
```C
#include <stdio.h>

int main(void){
	printf("String printed in console\n")
}

```
We can add "%s" to add variables inside the string like this: 
```C
#include <stdio.h>

int main(void){
	char variable[] = "Juan David"
	printf("Hello %s!\n", variable)
}
//Output: Hello Juan David!
```
The percentage sign is treated differently inside the formatted prints, so if we want to print a "%" then we have to use "%\%". 

Also there is a different value for "%" depending on the type of data which we want to plug in, for example: 
+ %s : string
+ %d : integer 
+ %c : single char/ character
+ %f : float values
	+ we can add the decimals precision: %.20f
+ %li : long integers
+ %i : integer
+ %p: pointer (memory address)


## fprintf

It allows us to print things as printf but on a file.

# Reading

## scanf

it allow us to read the users input in the terminal, it receives a string which indicated it what to read, and a direction where to store it. 

```C

int c;

scanf("%i", &c);

```

## fopen

It allows us to open a file, it returns the direction in the hard drive of the file, once we don't need it anymore we use fclose()

```c
#include <stdio.h>

FILE *file = fopen("nameofFile.csv", "mode");

fprinf(file, "%s", "text");

fclose(file);

```


# Sources
[Documentation](https://devdocs.io/c/io)