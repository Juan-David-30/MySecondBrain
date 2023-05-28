Related topics: [[Computer Science]], [[How to represent information]]

The precision of the decimals isn't complete accurate, and this is because of the translation from decimal to [[Binary]] system, it happens very often that we have recurring decimals, just like it happens in the decimal system: 

$$1\div3 = 0.\overline{3} $$
we have infinite 3 numbers after the decimal point, now we understand the recurrence and if we do this:
$$0,\overline{3}\times3 = 0.\overline{9} = 1$$
Now it turns out that the computer do not understand recurrence, rather they just limit the number of decimals and operate with them, the example above made by a computer (supposing that they could use decimal system) would be as follows:

$$1\div3 = 0.3333333333333333333333333 $$
$$0.3333333333333333333333333\times3 = 0.999999999999999999999999$$
Now it happens that the computers don't use the decimal system, instead they use the binary, which is based in powers of then, and when we're working with this decimals is more often seen this kind of recurrent numbers, for example in 0.1 which isn't recurrent in decimal system, is recurrent in binary, like this example there is a lot of them, so what out computer does is take a exact precision of bits to represent the decimals, and when it achieves the boundary the rest of the number is cut off, making the number un precise. 

The more bits we use the more precise it'll be, but we always will have at least a diminutive imprecision because we can't chase the infinity of the recurrence.

# Source
[Source](https://www.youtube.com/watch?v=PZRI1IfStY0)