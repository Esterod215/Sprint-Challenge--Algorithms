1. a)  a = 0 # O(1)
    while (a < n * n * n): #O((n*n*n) -1) drop constants: O(n*n*n)
      a = a + n * n O(1)
- The runtime is O(n^3)
2. sum = 0 O(1)
    for i in range(n): O(n)
      i += 1 O(1)
      for j in range(i + 1, n): O(n)
        j += 1
        for k in range(j + 1, n): O(n)
          k += 1
          for l in range(k + 1, 10 + k): O(k)
            l += 1 O(1)
            sum += 1 O(1)
- O(n^4) runtime

3.  def bunnyEars(bunnies): O(n)
      if bunnies == 0: O(1)
        return 0  O(1)

      return 2 + bunnyEars(bunnies-1) O(n)
- O(n^2) runtime

part II

- Divide n floors by two before you start looping
- check to see if egg breaks if thrown out window
-if it does divide in half again, and check if egg breaks.
-if egg did not break divide again until egg breaks at midpoint.
-start another loop and go downward until you find the floor that the egg doesnt break and the answer would be index plus 1.

there would be an initial loop that would half the floors and the a second loop that checks to see when the egg doesnt break
Runtime complexity would be O(nlog(n))

