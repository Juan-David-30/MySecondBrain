---
Tags: programmingLanguage 
Topic: Embedded-systems
---
Related topics: [[Computer Science]], [[Programming]]

C is a [[Compilers|compiled]] [[Programming languages|programming language]] which is a mid-level (between high level and low-level language) [[Programming languages#By its typed|static typed]], making it fast and efficient like for example for [[Embebed systems]]. And is also the language on which other languages are build. 

# Fundamentals

Once we write a program in C and now we want to run it, what we have to do first is use or run the compiler on our [[Source code]], the compiler will create a new file with the code translated to [[Machine code]] and then we will be able to execute it by putting its name in the terminal. 

+ Harvard [[CS50X]]
	In C the compiler is triggered by the command "make" followed by the name of the file where is the [[Source code]] which we want to [[Compilers|compile]]. 
+ Mac
	Mac has a compiler with itself so what we have to do is execute it through the command cc or gcc and then the name of the file which we want to compile, also we can use the flag -o and with it give first the name which we want to give to the compiled program (in assembler language) and then the file which we want to compile. 
	
	When we're working with third party libraries, isn't enough with using the header, we also have to tell to the compiler to look for the file where all this code is safe, and to do that we use the flag -l\<nameOfLibrary>. 
	
	For example when we're running the command make in CS50 IDE what it is truly doing underneath the hood is running the command of compilation (clang) with the flag of output (-o) and with the flag "-lcs50".

Hello world: 
```C
#include <stdio.h> // Needed to use functions like printf()

int main(void)
//The function that will be automatically executed once the program is run 
{
	printf("Hello world\n"); // Print formatted
}

int main(int argc, char[] argv[]);
//argc = argument count, argv = argument vector
//It allows us to receive arguments from the command line
```

+ ## Main
	Main as it name says is the principal function of C, and there we write all the principal logic of our program, or at least what will be executed once we run it.  
	```C
	int main(){
		// Our code
	}
	```
	Here you can notice that it is a function with a return of "int", and that's because, indeed it returns a int, but it is "invisible" for the user, and it represents a code of status, you can learn more about it in **error handling**. 
	
	Also we got to know that there is a way to access to different "flags" or values received when we run the script on the terminal. To do so we just have to add the following params: 
	 ```C
	int main(int argc, char *argv[]){
		// Our code
	}
	```
	
	Here "argc" stands for "argument count", and as we can notice we it is a integer which represents the number or quantity of arguments sent when we ran the program. 

+ ## Headers
	The headers are a important concept in C, it turns out that we have a bunch of different pre-made functions inside C, like in any other programming language, but C for optimizations purposes and because of being a "middle-level" language instead of a high-level.
	
	Therefore we have to specify which group of functions we want to include or use, and we do that through the headers, including a header means or tells to the computer to look for a file in the computer which contains the functions which we want to use. [C documentation](https://devdocs.io/c/)
	```C
	#include <header>
	```
	+ ### [[<stdio.h>]]
	+ ### <stdbool.h>
		+ allows us to use boolean expression such as true of false
	+ ### \<string.h>
		It has a bunch of function related with the management of strings, for example the function strlen() which returns the length of a string (something pretty useful).
	+ ### \<ctype.h>
		This is a library useful to perform case functions and operations, for example we know that the numbers map a number, but how do we for example map them to its upper case and lower case version, well if we see in ASCII we can notice that its upper case version always is 32 values separated to the lower case version, so if we subtract 32 to the lower case character, well get the upper case, an vice versa. 
		
		We can understand all this logic, but rather than doing all this manually we could use a library, and for this kind of problems we can use the **ctype** library. 

+ ## [[Comments]] 
	```C
	//Unique line comment
	
	/*
	
	Multiple lines comment
	
	*/
	``` 

+ ## [[Variables]]
	C being a programming language statically typed obligates you to set the [[Data type]] which the variable will contain before the name of the variable, then the name of the variable and the assignment operator "=", lastly on the right of the operator the value which the variable will contain closed with a semicolon(;)
	```C
	char *variable = "Value";//For a string we use a char array and doble quotes
	char c = 'C'; //For a single character we use char and single quotes
	int variable2 = 10;
	float variable3 = 12.2; 
	//So on
	const int n = 3;  //Creating constant
	```
	We can create a constant with the keyword const, so we can't change the value in the future and we can protect ourself of induced values. 
	We can also create variables, but not assign values: 
	```C 
	char variable; //Declaration of the variable
	variable = "C"; //Assign variable, notice we don't specify the data type again
	int variable2 = 2;//Initializate variable, both above together
	```
	[More information about the data types](https://byjus.com/gate/data-types-in-c/#types-of-data-types-in-c)
	
	We can create constants or "**Magical numbers**" that will be replaced anywhere in the code as follows: 
	```C
	#define CONSTANTNAME Value 
	```
	Now we can use the constant name anywhere in the code, and when we compile it will be replace for the value which we give it, hence if we have to do a change to that number we do it just once in the whole code. 
	+ ### Scope
		The scope is the characteristic of a variable to be accessed in certain context or block of code. 
		+ global scope: are the variables which can be accessed anywhere in the whole program. 
		+ Local scope: are the variables which can be accessed just within the function where they're declared. 

+ ## [[Arrays]]
	We can create a array as follows: 
	```C
	dataType array[length];
	int scores[3];
	scores[0] = 1;
	scores[1] = 2;
	scores[2] = 3;
	//To inicializate the array we can do the following: 
	scores[3] = {1,2,3};
	//We also can ommit the size, so it is set automatically 
	```
	The arrays aren't pass by value, instead they're pass by reference, it means that if we send them through a function, we have the actual array, so we have to be careful modifying it. 

+ ## Struct
	Struct is the way that C provide us to create different [[Data structures]], we already have some primitive [[Data type|data types]] and in base of them we can create structures with those primitives, indeed the [[Arrays]] are a "light" way of data structure where all the related data is back-to-back. 
	
	But what if we want to create certain data structures, for example if we for our [[Algorithms|phone book]] want a data structure which stores a person's name and phone number? Well we can create our own data structure as follows: 
	
	```C
	typedef struct
	{
		char name[]; //We can't default set values
		char number[];
	}
	person;
	```
	
	The sintaxis is very descriptive and it tells us that were defining something of type structure (so we can add multiple elements or structures inside it) the structure itself and ended by the name of the structure, once we've called this we can use the new data structure henceforth. 
	
	```C
	person people;
	people.name = "Name";
	people.number = "Number"; 
	```

+ ## [[Conditionals]]
	The conditionals are set with the reserved keyword "if", followed by the [[Boolean expressions|Boolean expression]] surrounded by "()" and finally with the causal surrounded by "{}".
	```C
	if (booleanExepression){
		//causal
	}
	```
	We also can use the "else" keyword to add a second causal, and even we can mix it with more boolean expressions as follows: 
	```C
	if (booleanExpression)
	{
		//Firs causal
	}
	else if (secondBooleanExpression)
	{
		//second causal
	}
	else
	{
		//Last causal, executed in case that none of the above is true
	}
	```
	The [[Logical combinators]] in C are used as follows:
	+ || : or (Inclusive) $\vee$  
	+ && : and $\wedge$ 
	+ !: not $\neg$  
	As in many other programming languages we can use a alternative to the common if conditional when we have multiple branches or options, and that's the switch structure:
	```C
	int x = get_int(); //CS50 function, do not use in actual code
	switch(x)
	{
		case 1:
			//code
			break; //Important to break, other wise it'll still going through
		case 2:
			//code
			break;
		case 3:
			//code
			break;
		case 4:
			//code
			break;
		default:
			//code
	}
	```
	Assigning a value we can also use this conditional: 
	```C
	int variable = (expression) ? 4 : 5;
	```
	if the expression is true, then variable will take the value of four, otherwise it will be 5.

+ ## [[Functions]]
	The functions as in the most of the programming languages are called or executed with the name of the function followed by parentheses and inside them the arguments or inputs of the function.
	
	We can also create our own functions as follows: 
	```C
	dataTypeOfReturn nameOfFunction(void)//we use void if we don't want to receive any argument. 
	{
		//Algorithm or logic of the function
		return returnedValue; 
	}
	```
	When we define a function and we want to use it before it is actually written, we have to include its "prototype" before where we're going to use them. 
	```C
	//This is the function prototype
	int nameOfFunction(char *parameters); 
	```

+ ## [[Operators]]
	We can do a bunch of things with a [[Computation|computer]], and its name indicates, it is useful to do computations, such as additions, subtractions, divisions, multiplications, and so forth. To tell to the computer to do any of these operations, then we have to use operators, in C we have the following ones: 
	
	Arithmetic operation: 
	+ A **+** B: addition
	+ A **-** B: subtraction
	+ A **/** B: division
	+ A **\*** B: Multiplication
	+ A **%** B: Module (Getting the remainder of division)
	+ ...
	When we operate with them we can encounter different error or imprecisions, those imprecisions can be mainly related to the use of [[Binary]] to represent numbers: 
	+ [[Integer overflow]]
	+ [[Truncation]]
	
	Assignment operator, in C and in computer science contest in general unlike in pure mathematics context we don't use the "=" as symbol of equality, instead is the assignment operator, it indicates to assign the right value or statement to the left value: 
	
	int variable **=**  4;
	
	the left variable will now storage the right value. When we call variable will be calling the value assigned, which is 4. 
	
	We can mix the arithmetic operators with the assign operators and it works as a sort of shorthand: 
	variable **=** variable + 1;
	variable **+=** 1;
	
	When we're adding or subtracting one unity we have the next shorthands: 
	variable **++**;
	variable **--**;
	
	Of course we can also use relational operators and [[Logical combinators]] to create [[Boolean expressions|Boolean expression]], such as the followings:
	
	Logical operator (logical combinators);
	+ && - [[Logical combinators#And (∧ &)|and]]
	+ || - [[Logical combinators#Or|or]] (Inclusive)
	+ ! - [[Logical combinators#Not (¬)|not]]
	
	Relational operators: 
	+ > - greater than
	+ < - less than
	+ <= - less or equal than
	+ >= - greater or equal than
	+ == - equal to
	+ != - different to
	```ad-info
	The comparation of two strings can't be done with the doble equal sign,
	instead we have to use a funcion of the string library called strcmp()
	```

+ ## [[Loops]]
	 + While
		As in many languages we can use the while loop where we ask a question multiple times, and will repeat the block of code inside the "{}"  until the condition stop being true, so we have to make sure that there is a point where that condition will be broken, otherwise we can make a infinite loop and saturate our CPU. 
		```C
		int counter = 3;
		
		while (counter > 0)
		{
			printf("Hi\n");
			
			counter--;
		}
		```
		If we want to create a infinite loop just like in [[Scratch]], we can use the following logic:
		```C
		while (true) // we can also use while (1)
		{
			//code executed forever
		}
		```
		We can break loop, either infinites and finites, with the break keyword
		```C
		
		while (true) // we can also use while (1)
		{
			break; //Will break the loop, so isn't completely infinite
		}
		```
	+ For
		As in other programming languages we can use the for loop, which receives 3 values separated for semicolons, the first is the variable of control, second the condition that will be ask after each iteration, and at last the operation applied to the control variable to avoid infinite loops: 
		```C
		for (int i=0; i<3; i++)
		{
			//Code executed multiple times
		}
		```
	+ do-while
		do-while is a loop which ask executes the block of code first, and then ask the question, then we can ensure that the code will be executed at least once, and henceforth will be executed just if the condition is true: 
		```C
		do
		{
			//Code to be executed
		}
		while (BooleanExpression);
		```

+ ### [[Error handling]]
	In C we don't have explicit or specific sintaxis for that, rather we use return values, and if we notice it turns out that the main function always has a "int" as return value, and indeed it does return a value, commonly is hidden, we can see the value that returns by running the command "echo $?". 
	
	By default it returns 0, but we can return any value, and thanks to that we can kinda error handling by stoping the program and sending a number as sort of a "code". 

+ ## [[Pointers]]


# [[Frameworks]]
```dataview

TABLE FROM #framework 
WHERE contains(Language, "C")

```

# Documentation
[C documentation](https://devdocs.io/c/)