---
Tags: DataStructure
Alias: Array
---
Related topics: [[Computer Science]]

An array is a way in which we can storage data back-to-back in the [[Memory]], so we don't have to create multiple individual variables, instead one which ask for the necessary space to save them all and then we index them by numbers, counting from 0. 

Here a example of a array: 

```C
int scores[3];

scores[0] = 1;
scores[1] = 2;
scores[2] = 3;

```

 Here we can see how we have sorta three variables in one. But the advantage is that is more scalable and correct, using this we could for example use loops.
 
```C
int scores[3];

for (int i = 0; i < 3; i++)
{
	score[i] = i + 1;
}
```

The arrays are pretty useful, and indeed the [[Data type]] string, isn't more than a string of **chars** or characters, indeed in [[C]] we don't have a string data type, instead we use a char array[], what's exactly that, a array of characters.

Now, something interesting happens always with the string, and that's that the computer doesn't know where to stop reading a string, where that array of chars ends, so o declare that, we always have one more bit, which is exactly a 0 (ASCII mapped to NUL), and it tells to the compiler or computer that there is where the string ends. 