# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0    O(n) Linear
    while (a < n * n * n):
      a = a + n * n
```


```
b)  sum = 0
    for i in range(n):
      j = 1            O (n log n) O linear & logerithmic
      while j < n:
        j *= 2    
        sum += 1
```

```
c)  def bunnyEars(4):  O(n) linear
      if bunnies == 0: 
        return 0    

      return 2 + bunnyEars(4-1)
```

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

1.) Create a bianary tree where the root is the mipoint f is the root 

          n = [number of floors]

          start = 0
          end = 0
          midpoint = start + end //2

            midpoint floor
if f< mid   /           \  if f> mid 
f goes left                  f goes right
       
       when tree reaches the leaves then return the smallest number