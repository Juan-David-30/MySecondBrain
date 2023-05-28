---
Alias: Matrix
---
Related topics: [[Mathematics]]

# What's a matrix?

A matrix $A_{mn}$, is a set of data arranged throughout m rows and n columns, it can be described as a rectangular array or table of [[mathematical objects]] or a property of a object. The factor m$\cdot$n is known as the dimension of the matrix.

![[Matrix example.png]]

# What are they useful for?

The matrices has multiple applications in [[Mathematics]], [[Computer Science]] and [[Physics]], for example in [[Computer Science]] we can use them in a way of [[Adjacent matrices]] to represent graphs in graph theory, in which each cell of the matrix represent whether exists a edge from m to n. 

In [[Physics]] is pretty important too, they are present for example in [[Thermodynamics]], [[Electromagnetism]], fluid mechanics, the relativity theory and so on. 

# Types of matrices

## Square matrix 
Is a matrix which has the same amount of rows and columns (m = n)

## Row matrix
Is a matrix 1 $\cdot$ n which has just one row and multiple columns 

## Column matrix
Is a matrix n $\cdot$ 1 which has just one columns and multiple row 

## General matrix
Which is the matrix of the way m $\cdot$ n where m n can be different to zero and m can be different to n. 

# How to operate matrices

## Addition and subtraction

When we're adding two matrices we first have to make sure that they're dimensions are the same, otherwise we wouldn't be able to do that. 

A + B $\lor$ A - B  $\implies$ dim(A) = dim(B)

To add or subtract matrices what we have to do is add or subtract all the positions, so the element 1,1 of A with the 1,1 of B, and then the 1,2 of A the 1,2 of B and so on. 

## Multiplication

Multiplication of a matrix for a constant factor, what we have to do is multiply the factor for each element of the matrix. 

Multiplication of two matrices, firs we have to realise about some things, first the number of columns of the first operand must be the same to the number of rows of the second one:
$$A_{mn} \cdot B_{m'n'}\implies n=m'$$

Also we must notice that the multiplication between matrices doesn't have the commutative property
$$A_{mn}\cdot B_{m'n'} \not = B_{m'n'}\cdot A_{mn}$$
Now, when we multiply two matrices the product will be a new matrix with the number of rows of the first operand and the number of columns of the second operand: 

$$A_{mn} \cdot B_{nr} = C_{mr}$$

And the what we have to do is multiply each row of A, by each column of B and sum the products. 
$$C_{ij} = \sum_{k=1}^{n} A_{ik}\cdot B_{kj}$$
In this multiplication we can encounter with a extremely peculiar matrix, which is known as the identity matrix, is a matrix which when is multiplied by other matrix the result will be the matrix which is being multiplied by, even if we flip the order
$$A_{nm}\cdot I_{mn} = I_{nm}\cdot A_{mn} = A_{mn} $$
This matrix is really peculiar because its elements has the following pattern:
$$\begin{pmatrix}
1 & 0 & 0 & \ldots\\
0 & 1 & 0 & \ldots\\ 
0 & 0 & 1 & \ldots\\ 
\vdots & \vdots & \vdots & \ddots
\end{pmatrix}$$
Is a matrix full of zeros but for its diagonal where there are ones.  


## Transpose

To transpose a matrix what we have to do is sort of "Rotate" the matrix where we convert the columns intro rows and vice versa:

$A_{mn}^{t}=A_{nm}$
