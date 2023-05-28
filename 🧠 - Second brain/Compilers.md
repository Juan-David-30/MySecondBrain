Related topics: [[Computer Science]]

The compilers are programs responsable to translate a [[Programming languages]] into [[Binary]], the compilers unlike the [[Interpreters]] translates the code just when it is written, so when you finish of writing a code, you have to run the compiler which translates it to [[Binary]]  and creates a new file with that Binary code. Of course having some advantages like the being faster at the execution moment.

Now let's understand a little better the process that this programs follow to compile your code:

# Compiling process

## preprocessing 

Always when we run the compiler on a file with [[source code]], first it does a preprocessing, there is some lines which has to be processed before the others (this lines has are preprocessor directives).

for example in [[C]] all the lines which start with the "#" symbol will be preprocessed, and those could be the magic number (replacing each part in the document when the keyword appears). 

Or the include lines which defines a header, the compiler will look for the files which those headers specify in the "/usr/include" direction and will sort of copy and paste the information of that file where you wrote the header. 

## Compiling

This is the step in which the compiler literally compiles or translates your code, more specifically to [[Assembler]] language.

## Assembling

Once the computer has translate your [[Source code]] to [[Assembler]], what it does is assemble it, what is literally translate the assembler to [[Binary]], something that can be already understood by the [[CPU]]. 

## Linking 

Although the code that we've written is already translated to [[Binary]], one last step is missing, and that step is linking the code that we wrote, with the other libraries specified in the headers, so the las step is grab the [[Binary]] of each document, and finally putting them all together. 

---

# Decompiling 

Decompiling is indeed possible, we can return from zeros and ones to a higher level programming language, now it would be pretty hard to understand for several reasons, and first, all the style would be of course lost, all the names to variables and functions would be lose and probably named of a not understandable way, and there is a some logics which logically do the same so they'll be compile in the same code, to decompile that would be very hard to know exactly which representation is the original one. In resume would be a complete mess. 