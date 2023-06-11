---
Topic: ComplexNumbers
---
Related topics: [[Complex numbers]]

The operations or functions on these new sort of numbers are studied by the arithmetic, specifically the complex arithmetic is the branch of arithmetics devoted to study these mostly binary functions and properties of the complex numbers. 

# Complex conjugates

In the complex arithmetic the complex conjugates play a actually interesting and useful role, as we've mentioned above, the complex numbers can be thought as a number with two parts or even two terms, the real part and the imaginary part, so as if it is a binomial we can conjugate them: 
$$ z = a +bi$$
The conjugate of the number z, is as follows:
$$ \bar{z} = a -bi$$
The conjugate is commonly represented either with a bar over the letter as above, or with a star(\*). 

If we plot both number on the complex plane, we'll notice that they're the same but reflected or mirrored over the real axis. 
![[Real conjugate.png]]
These conjugates has some interesting properties, for example if we add to a number its conjugate we'll get its real part twice: 
$$ z+\bar{z} = 2\cdot Re(z)$$

But what is even more interesting is the multiplication, when we multiply a complex number by its conjugate we'll get its magnitude (or module) of the complex number squared. 

$$ z \cdot \bar{z} = \lvert z\lvert^{2}$$
# Divide complex numbers

To divide the complex numbers, we have to make use of the conjugate, specifically of the conjugate of the denominator, so what we got to do i multiplicate the expression by the conjugate of the denominator over the conjugate of the denominator: 
$$\frac{z_{1}}{z_{2}}\cdot\frac{\bar{z_2}}{\bar{z_2}}$$
So we don't have any imaginary number in the denominator, and we can operate the rest of the process easily. 

# Absolute value 

To find the absolute value of a complex number, we have to visualize the complex plane, and the coordinate which it presents, then we have to retrieve the definition of the absolute value, which is the distance between the origin point (0,0) and the number, so to find the absolute value of a complex number we can do it through thinking the real and imaginary part as the legs of a triangle and the absolute value as the hypotenuse of that triangle, then finding it thanks to the pythagorean theorem. 

![[Absolute value complex numbers.png]]

# Multiplication graphically

We can think in the multiplication algebraically and graphically, algebraically we just have to thing the complex numbers as a binomial and start operating with the distributive properties and so on. But the most interesting part is the graphically way, in which we can notice of some patterns and interesting behaviors.

Indeed the graphic multiplication, is based on the [[Polar coordinate system]] rather to the commonly used, where instead of taking the value of each axis what we do is take the a distance respect to the origin coordinate and an angle. In this system we get that 

$$r_1(\cos\theta_1+i\sin\theta_1)\cdot r_{2}(\cos\theta_2+i\sin\theta_2)$$

Associative property of multiplication: 
$$r_1r_2(\cos\theta_1+i\sin\theta_1)(\cos\theta_2+i\sin\theta_2)$$

Now we solve for the parentheses: 
$$ r_1r_2 (\cos\theta_1\cos\theta_{2}+i\cos\theta_1\sin\theta_2+i\sin\theta_1\cos\theta_1-\sin\theta_1\sin\theta_2)$$

Let's rearrange them and group them:
$$ r_1r_2 ((\cos\theta_1\cos\theta_{2}-\sin\theta_1\sin\theta_2)+(i\cos\theta_1\sin\theta_2+i\sin\theta_1\cos\theta_1))$$

We can identify the [[Trigonometric identities]]: 
$$r_1r_2(\cos(\theta_1+\theta_2)+ i\sin(\theta_1+\theta_2))$$

But the interesting part of all this process is that we can simplify it by thinking that what we just do is adding the angles and scaling (multiplying) the modulus or absolute values. Making all this process easier.

Dividing is similar, you can do all the algebraically and we'll find out this: 
$$\frac{r_1}{r_2}(\cos(\theta_1-\theta_2)+ i\sin(\theta_1-\theta_2))$$
here we can notice how we just divide the modulus and subtract the arguments. 

# Powers of complex numbers

Now we have the bases to find the powers of complex numbers, and even the roots of complex numbers, now we know that when we multiply a complex number by other one what we're doing is adding their arguments and multiplying their absolute values or modulus. 
$$z^{n}= |z|^{n}(\cos(arg(z)\cdot n)+i\sin(arg(z)\cdot n))$$

And if we want to find the root of these numbers we can logically do the opposite process: 

$$  \sqrt[n]{z} = \sqrt[n]{|z|}(\cos(\frac{arg(z)}{n})+i\sin(\frac{arg(z)}{n}))$$
Here what we're doing in finding the modulus which multiplied by itself n times will return the modulus of z, and we're finding the angle which multiplied by n, will return the angle of the complex number, it makes sense of course, but we can notice that it's of course not the unique solution, there are more solutions, knowing that the $arg(z) = arg(z)+2k\pi$, being k any integer number. 

So we can find more complex solutions, indeed there are infinite angles, but how many of them represent different solutions?, because we can have two numbers which look different in its polar form, but their the same in it's rectangular form. 

Well here is where the [[Fundamental theorem of algebra]] pops out, and it turns out that $z = \sqrt[n]{-x}$ is the same as $z^{n}=-x$, so this is a equation, and the theorem tells us that each equation has the same number of solutions in the complex numbers as the grade of the polynomial. So the $\sqrt[n]{z}$ will have n solutions. 

And how do we find them?, just using what we got about, and using the mode $arg(z)+2k\pi$, and taking all the whole values of k, starting from 0 and ending at n-1. 

And what's more interesting about this is that all these solutions returns a perfect polygon which numbers of sides is n. 

![[Set of solutions of fifth root of (1).png]]