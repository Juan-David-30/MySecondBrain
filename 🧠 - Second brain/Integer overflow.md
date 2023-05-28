Related topics: [[Computer Science]], [[How to represent information]]

Integer overflow is a phenomena or error which we can encounter when we're operating or working with integer numbers on a computer. 

it turns out that the computers use [[Binary]] of way to interprete information, and of course numbers as the integers, but we have a sort of trouble here, and it happens that the [[Memory]] of the computers of course is limited, so we have to define a exact number of bits for the number, for the integers in languages as [[C]] it is limited to 32 bits, in other words 4 bytes. So if we put all the bits in 1.

The highest number which we can storage or represent is:

4294967295

But we commonly use the integers to represent not just positive, but negative values, so we use half of the patterns to represent positive numbers, and have to negative, so the highest and lowest are: 

Highest: 2147483647

Lowest: -2147483648

Right, now let's see what happen when we try to represent higher values than the limit, what will happen is a **Integer overflow**.

We'll try to add a value longer to: 11111111111111111111, what we'll need is to add a new bit: 
**0**11111111111111111111 and then we'll have: **1**0000000000000000000000.

That's how ideally it should work, but in the reality we'll find out that as said we have a fixed amount of bits for each integer, so what will happen is that well change all the value to:
**1**0000000000000000000000, but we actually don't have the extra bit, so what we'll have is: 
0000000000000000000000, so we've overflowed the integer, is like we have restarted the count, and it is worst know that the half of the values are negatives, so instead of getting: 

2147483647+1 = 2147483648

we'll get: 

2147483648+1 = -2147483648

To avoid this, the obvious solution is to use a longer number of bits, and to do that for example in c we have the "**long**" [[Data type]] which doesn't give us 32 bits, but 64, doubling the number of bits and giving us a larger boundary. (Of course if it isn't enough in case that we're working with really long values, then we have to use longer quantities of bits, be aware that we'll always have physic limits), We can also use the "**unsigned int**" which is the same int value (32 bits) but all the possible values are used to the positive numbers, so we don't have to split them between negatives and positive numbers, we just have positives. 