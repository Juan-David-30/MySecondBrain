---
Tags: Concept
---
Related topics: [[Mathematical logic]]

To become more precise with our [[Mathematical language]], the [[Mathematical logic]] has set or defined strict, precise and unambiguous meaning to the different connecting words.

The logical combinators are words which allows us to as its name indicates to combine multiple statements, and then give them a logical meaning such as them both are or have to be true, either of them has to be true or both, and so on. 

# And (∧ &)

And is a logical combinator which allows us to combine two statements in a way that both have to be true or apply for this case. 

```ad-example
π is bigger than 3 **and** less than 3.2

(π > 3) **&** (π < 3.2)

```

If we have the statements  ø and µ: ø ∧ µ means that both ø and µ are true conjunction.

ø, µ are called the conjuncts of ø ∧ µ.

So if both conjuncts (ø and  µ) are individually true, the conjunction will be true, other wise if either ø or µ is false or even both are, the conjunction will be false.

+ Truth table
	![[Truth table and operator.png]]

The conjunction follows the **Commutative** so: 

ø ∧ µ = µ ∧ ø  (Think that not always happen in natural language)

# Or

Or is a logical operation which has the logic of say that either one or other statement can be true, but it can have two uses: 

```ad-abstract
title: Exclusive or
a > 0 **or** the equation x^2 + a = 0 has a real root  

```

Here either of the statements can be true, but not both at the same time, so is exclusive, if one is true, then the other isn't. 

```ad-abstract
title: Inclusive or
ab = 0 if a = 0 **or** b = 0

```

Here again either of the statements on the both sides of the or can be true, but in this case they both can be true, so is inclusive. 

In natural language we can use the exclusive and inclusive way with the same symbol, but it can generate some ambiguities so to avoid it in mathematics we have a symbol for each one: 

+ ## Disjunction (Inclusive or)
	For the inclusive or we use the "∨" symbol also known as the disjunction symbol. 
	ø,  µ : **ø ∨ µ** means ø or µ (or both):
		called the disjunction of ø and µ
		ø and µ are called the disjuncts. 
	
	Remember a disjunction means that at least one of the disjuncts has to be true or them both. 

+ ## Exclusive disjunction (exclusive or)
	For the inclusive or we use the "⊻" symbol also known as the disjunction symbol. 
	ø,  µ : **ø ⊻ µ** means ø or µ (not both):
		called the disjunction of ø and µ
		ø and µ are called the disjuncts. 
	
	Remember a disjunction means that at only one of the disjuncts has to be true. 

# Not (¬)
The not operator is used to negate the statement next to the not, is represented by ¬ or by ~. 

¬ ø
	if ø is true, then ¬ ø is false.
	if ø is false, then ¬ ø is true.

sometimes we use other symbols to specific operations or relations such as 

+ ≠ different or not equal to, we could represent it as ¬(=)
+ ≯ not greater than, we could represented as ¬(>)

But we sometimes have to prefer using the ¬ symbol rather than those alternatives to avoid ambiguity. 


# Sources
[[Introduction to mathematical thinking]] - Stanford online