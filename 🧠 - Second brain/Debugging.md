---
Tags: Concept
---
Related topics: [[Computer Science]], [[Programming]]

When we're programming and creating [[Algorithms]] often we'll encounter some mistakes, a large sort of mistakes, some of them obvious like sintaxis ones, you forgot to add a semicolon (;) so on. 

But there is other which are harder to notice, or to encounter, they're more subtle, and probably they're logic ones, so how can we encounter them and solve them?, we'll probably we can ask someone, look for help, search in internet, there is a lot of options and they're all valid. But it would be better if we start to develop or acquire our own tools, so we can solve them by our selves. 

# Debugging tools

there is a lot of tool which we can use to somehow inspect the working of our program: 

## Print

This is the most basic one, but it still being pretty useful, it consist in using or printing values on the screen, so we can check the step-by-step, for example checking how many times a [[Loops|loop]] is being printed, what's the current value of a [[Variables|variable]] in a specific step, and so on. 

## Debugger

When we're debugging some times the process of printing can become tedious once the program is long and we have to run it all to see the specific print and so on. 

So instead we can tools to debug our code, for example visual studio code has its own debugger tool. 

When we hover on a line of code a red point will appear in the left side of the line. If we click it it’ll be set as a breakpoint and will stay red even when we don’t hover it.


### What's a break point? 

When we use a editor or IDE a breakpoint is a mechanism which allows us points or lines we want to stop the execution and get the data and poke around the functioning of the specific line of code.

### How can we control the execution? 

Once we’ve set the breakpoints and start running the debugging will get the following menu:

-   First button is for jumping toward the end of the execution (like finishing it) or for jumping into the next break point
-   Second one is to step over like execute it but not diving into it.
-   Next is step into which dives into the execution of each step, so instead of just executing it, it’ll go to the function and see the step by step of what is being executed.

### What can I see when executing?

Whilst we’re executing the debugging a new section will appear in out window named variables, There again will have two new sections named local and globals in which will appear the variables with its assigned value depending of its scope.

## Rubber duck 

Is a funny but useful technique which consist in explain your code or logic to a rubber duck verbally and loud, therefore we may probably realize of the mistake or our logic error while explaining it. (A rubber duck isn't necessary we can talk with someone else or even to your self).

# Sources
[[CS50X]]