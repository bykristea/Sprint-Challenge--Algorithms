#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)a = 0 --> constant so O(1)
while (a < n _ n _ n): --> O(n)
a = a + n \* n

O(1) + O(n) = O(n)

ANSWER: O(n)

b) sum = 0 --> O(1)
for i in range(n): --> O(n)
j = 1
while j < n: --> 0(n)
j \*= 2
sum += 1

ANSWER: O(n^2)

c) def bunnyEars(bunnies):
if bunnies == 0:
return 0

      return 2 + bunnyEars(bunnies-1)

      ^runs one function for n(bunnies). re-calls function each time decrementing by 1 until reaching 0

      ANSWER: O(n)

## Exercise II

I think a Binary Search would work for this scenario. Start with the middle floor and drop an egg. If it breaks all floors above can be ignored/ruled out. Then move your low, mid and high points to test the bottom half. If at the new mid it breaks, you rule out the upper floors and vice versa. Repeat until we find a floor that the egg doesn't break at at and the floor directly above does break.
