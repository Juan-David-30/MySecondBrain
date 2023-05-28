Related topics: [[Trigonometry]], [[Trigonometric functions]]

The trigonometric identities are equations that involve [[Trigonometric functions]], but which apply for all the cases, so it means that no matter the context we can apply them an they stay true, for example the equation x+1 = 8, is a common equation, but not a identity, because this applies just for one value, but what about |x| = $\sqrt{x^2}$, here we have an identity because it applies for all the cases or values which x can take. 

# Symmetry

## sine and cosine

taking as reference the [[Unit circle]] we can notice that we can get some symmetries when we're working with different angles:

![[Symmetry on unit circle.png]]

Here we can notice that there are a lot of different angles in which the sin and cosine values are the same, even though the angles are in principle different, and that's because of a symmetry, we can notice how for example sin($\theta$) = sin($\pi-\theta$), and that's the same angle or triangle but reflexed by the y axis, and being sin the value of the y axis, stays the same. 

But notice how we can also say that cos($\pi-\theta$) = -cos($\theta$), they have exactly the same absolute value but they're opposite because of the reflexion respect to the y axis, know if we reflex the angle by the x axis we would have the opposite case, in which the cosines has the same value while the sines has the opposite value (stay having the same absolute value) and if we reflex respect the origin point both would be opposite, but stay important to notice of this symmetry. 

In the next table all the values in the same row has the same value:
| First sector  | Second sector      | Third Sector       | Forth sector                          |
| ------------- | ------------------ | ------------------ | ------------------------------------- |
| sin($\theta$) | sin($\pi-\theta$)  | -sin($\pi+\theta$) | -sin(2$\pi-\theta$) / -sin($-\theta$) |
| cos($\theta$) | -cos($\pi-\theta$) | -cos($\pi+\theta$) | cos($2\pi-\theta$) / cos($-\theta$)   |


## Tangent

The tangent is the ratio of the sin / cosine, what can be alto thought as $\frac{y\Delta}{x\Delta}$, thinking of that way if we return to the unit circle:

![[Symmetry on unit circle.png]]

We can notice how the yellow and blue line are somehow continues, how they continue each other, and the same for the pink and green, so we can start noticing how the symmetry works for the tangent, even we can do the proves algebraically:

### Tan($\theta$) = Tan($\pi+\theta$)

We know that tan$\theta$ is the same as $\frac{sin\theta}{cos\theta}$, so tan($\pi+\theta$) = $\frac{sin(\pi+\theta)}{cos(\pi+\theta)}$ also we know that sin($\pi+\theta$) = - sin$\theta$ $\land$ cos($\pi+\theta$) = -cos$\theta$, so $\frac{-sin\theta}{-cos\theta}$ and that's equal to $\frac{sin\theta}{cos\theta}$ (for signs law) and that finally we have that it is equal to tan($\theta$).

We can do the same proof for the tan($\pi-\theta$) = tan($-\theta$), and we can notice that again all the absolute values of the different symmetries are equal so:
| First sector | Second sector      | Third Sector      | Forth sector |
| ------------ | ------------------ | ----------------- | ------------ |
| tan($\theta$)  | -tan($\pi-\theta$) | tan($\pi+\theta$) | -tan(-$\theta$) |

(All these values above are equal to each other).

# Periodicity

The periodicity is the property or phenomena of repetition, the symmetry by itself shew us some periodicity in the trigonometric functions through trigonometric identities, for example we know that sin$\theta$ = sin($\pi-\theta$) or that tan$\theta$ = tan($\pi+\theta$) and so on.

Know working in a circle, we can notice that if we start increasing the angle more and more, we'll just iterate over it, we'll return to the same spot, so for example cos$\theta$ = cos($\theta+2\pi$), this identity is obvious because is practically the same angle, we've just added a [[Angles#Type of angles|full rotation angle]] which is the same of the start, for that reason the [[Trigonometric functions]] are periodic. 

But we can find out other periodicity, not just in the same function but related between them, for example the periodicity of the sin and cosine.

Yeah the sin and cosine have a periodicity between them, let's see the following example:

![[Periodicity sin and cosine.png]]

Here we can notice that if we have a angle $\theta$ and we add to to it a right angle ($\frac{\pi}{2}$) what we're doing is rotate the triangle $\frac{\pi}{2}$ radians. So the qualities of its sides are the same, for the adjacent and opposite legs, but now if we notice in this caser the sin and cosine are "inverted" so we can say that cos$\theta$ = sin($\theta+\frac{\pi}{2}$) and the same for the sin, sin$\theta$ = cos($\theta+\frac{\pi}{2}$). 

So we can notice how there is a periodicity of the functions sin and cosine every $\frac{\pi}{2}$ radians. 

# Addition 

We also have some interesting and of course useful identities for addition in the angles of the [[Trigonometric functions]], let's see first the most important ones:

## $\sin(a+b)$

This is one of the most important ones, and from it we can get the most of them, of course here doesn't apply the distributive property, but we have something such as:
$$\sin(a+b) = \sin(a)\cdot\cos(b)+\cos(a)\cdot\sin(b)$$

This may look a little weird but actually it makes sense, it has multiple proofs, but my favourite is more of the style of geometry and analysis:  
![[proof addition identities.png]]

Here we can notice how the sin(a + b) is equal to the segment PQ, so to get it we have first to get the length of RS, which is $\sin(a)\cdot\cos(b)$, because if you notice the hypotenuse of a is OR, which is the adjacent leg of the triangle of the angle b, so to get that length we have to multiple, and to OR we must add PT, getting PT.

To get PT we have to imagine other triangle as we can see above in the graph, and after doing some angle hunting, and we finally find that the length of PT is equal to the cosine of a times the sine of b (which works as hypotenuse of this derivate triangle).

And we can do the same to find the identity of the cos(a + b) where we have to find the segment OQ (which would be the new adjacent side in the new triangle) is equal to OS-QS which can be found with the same idea planted before. 

To find the subtraction identities we can for example just think it as a addition where the second angle is negative, or we can also do the visual proof just as above planting a framework where we start from one angle and we subtract other. 

Now that we know how to find the basic trigonometric identities, let's set them in the next table: 

| Addition value | Identity                                        |
| -------------- | ----------------------------------------------- |
| $\sin(a+b)$    | $\sin(a)\cdot\cos(b)+ \cos(a)\cdot\sin(b)$      |
| $\sin(a-b)$    | $\sin(a)\cdot\cos(b)-\cos(a)\cdot\sin(b)$        |
| $\cos(a+b)$    | $\cos(a)\cdot\cos(b)-\sin(a)\cdot\sin(b)$       |
| $\cos(a-b)$    | $\cos(a)\cdot\cos(b)+\sin(a)\cdot\sin(b)$       |
| $\tan(a+b)$    | $\frac{\tan(a)+\tan(b)}{1-\tan(a)\cdot\tan(b)}$ |
|$\tan(a-b)$|            $\frac{\tan(a)-\tan(b)}{1+\tan(a)\cdot\tan(b)}$                                    |


## $\sin(2\theta)$

There are also a lot of identities coming from the double of a angle, all these identities are derived from others such as the adding identities specified above (and it makes sense because for example $\sin(2\theta)$ is the same as $\sin(\theta+\theta)$), and also from the Pythagorean identity ($\sin^{2}\theta+ \cos^{2}\theta = 1$). 

| Value       | Identity                |
| ----------- | ----------------------- |
| $\cos(2a)$  | $\cos^{2}a - \sin^{2}a$ |
| $\cos(2a)$  | $2\cos^{2}a - 1$        |
| $\cos{^2}a$ | $\frac{1+\cos(2a)}{2}$  |
| $\cos(2a)$  | $1-2\sin{^2}a$          |
| $\sin{^2}a$ | $\frac{1-\cos{^2}a}{2}$ |
| $\sin(2a)$  | $2\sin a \cdot \cos a$  |

