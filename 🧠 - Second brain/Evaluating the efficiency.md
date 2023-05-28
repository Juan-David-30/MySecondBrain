Related topics: [[Algorithms]], [[Computer Science]]

When we're working with algorithms we don't mind just for the correctness (which of course is important and fundamental) but also for it's efficiency, and we measure the efficiency of the followings ways: 

For example retaking the above's example of the phonebook, of course we can notice that this isn't the unique algorithm which can work for that situation (This is known as [[Binary search]]). 

Other example would be check page per page from the first to the last until we find it (This is known as [[Linear search]]). But of course we know that this is more slow, but why?, of course for small problems it may be fast and we won't notice about it, but the larger the problem is the longer it'll take to the algorithm to find what's looking for. We could try to go stepping two or three, four, and so on to make it faster, but we'll have the same graphic or behavior as the problem gets bigger. 

![[Graphic of algorithms efficiency.png]]

The red and yellow lines strokes are the [[Linear search]] representation of how long it takes to the algorithm to solve problems as the problem becomes larger. Whilst the green curve represents the behavior of the [[Binary]] search.

Notice how as the problem gets larger the [[Linear search]] takes that long that overflows the graph, whereas the [[Binary search]] stays really similar, or grows very slow, and it makes sense, because if you double the size of the problem, the [[Linear search]] would double it's time to solve or steps, while the [[Binary search]] would just increase one step more. 

# O (Upper bound)

In this examples we're measuring how a algorithm would perform in the "worst case", which would be the largest amount of time in terms of n which it would take to a algorithm to solve a problem, to do this measurement we use [[Asymptotic analysis]]. 

To represent this big O, we use the examples of above, but when we work with the big O value, we don't care about small differences such as n or n/2, for the big O notation they're the same, because as the problem is greater and greater they behave practically the same being a rect line pointing upwards (They have the same shape).  So we use the term "On the order of ..." and the general notation. 

Indeed we might say that this big O values are based in the general idea than in than in the specific reality. So for the algorithms n an n/2 they're the same as just n, and also for the [[Binary search]] algorithm which behaves as a logarithm function (log n).

![[Big O graph.png]]
 
We can have multiple big O values, like the following ones (sorted from slowest to fastest): 

O($n^2$)
O(n log n)
O(n)
O(log)
O(1) {A fixed amount of steps regardless the n value}

#  $\Omega$ (Lower bound)

The big O sort of specifies the upper bound or the highest amount of steps which can take to the algorithm to solve the problem in terms of n, whilst the $\Omega$ is used to set the lower bound, the "best" case. 

Again from slowest to fastest: 

$\Omega$($n^2$)
$\Omega$(n log n)
$\Omega$(n)
$\Omega$(log)
$\Omega$(1) {A fixed amount of steps regardless the n value}


In our both current examples [[Linear search]] and [[Binary search]] we have $\Omega$(1)

# $\Theta$ (O = $\Omega$)

Theta is used to indicate when a algorithm has the same lower and upper bound. 

$\Theta$($n^2$)
$\Theta$(n log n)
$\Theta$(n)
$\Theta$(log)
$\Theta$(1) {A fixed amount of steps regardless the n value}

For example if we want to count the people in a room and we use a linear algorithm of counting one by one, then in the best case it'd take us n steps, and in the worst case it'd take us the same n steps. 
