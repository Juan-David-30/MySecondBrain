Related topics: [[Mathematical logic|Formal logic]]

The quantifiers are used to express quantities, the "**there exists**" or "**for all**", these are pretty important due all the theorems and mathematical statements can be expressed just by using both. Being the there exist to specify that there is one object "x" with one property or for all to explain that all objects "x" has this property. 

# There exists

**There is** an object "x" having property "p". The there exists is represented by the symbol "$\exists$", let's see and example: 
$$\exists_x[x^3+3x+1=0]$$

Here we're saying that there exists one number "x" which in that algebraic expression is sufficient to preserve the equality. 

Often we want to more specific about the x, for example in the above's example saying that x has to be less than 0, we could just do this "$\exists_{x<0}$".

Other example of the use of there exists and specifying a value is the following: 

We want to prove that $\sqrt{2}$ is rational, so to do that we have to prove that there exist two natural numbers "p" and "q" such that $\sqrt{2} = \frac{p}{q}$.

The above's expression can be written as follows: 
$$(\exists_{p\in\mathbb{N}})(\exists_{q\in\mathbb{N}})[\frac{p}{q} = \sqrt{2}]$$

or even we can use a shorthand as follows:
$$(\exists_{p,q\in\mathbb{N}})[\frac{p}{q} = \sqrt{2}]$$

# Universal quantifier

The universal quantifier is the quantifier which allow us to say that for all the elements x the property p, and the symbol is "$\forall_x$" (for all x it is the case that...), example: 

"The root square of any real number is grater than or equal to zero"
$$\forall x(x^{2} \ge 0)$$ 
# Combination of quantifiers

We of course can of course make compound statements by mixing or combining quantifiers, for example:

"There is no largest natural number"
$$(\forall x\in\mathbb{N})(\exists y\in \mathbb{N})(y>x)$$
(For all the natural numbers there is a numbers which is grater)

notice that the order of in which the quantifiers are written in important, if we switch the order, the meaning would change: 
$$(\exists y\in \mathbb{N})(\forall x\in\mathbb{N})(y>x)$$
(There is a natural number which is larger than all natural number) 