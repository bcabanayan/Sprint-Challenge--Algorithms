Exercise I

a) The running time is O(n). The number of times the while loop runs depends on the value of n * n * n divided by the inner loop's n * n, essentially leaving O(n).

b) The running time is O(n^3). For every loop except the last, the number of time the function executes depends on n, and n must be multiplied by n for each nested loop. However, since the number of times the final loop depends on a constant, that term can ultimately be dropped as insignificant.

c) The running time is O(n). The final recursive loop indicates that the function will run based on the number of bunnies that are originally input into the function.

Exercise II

With an unlimited number of eggs, it makes the most sense to divide the the number of floors _n_ by 2, and then to throw the first egg off of the floor that is equal to _n_ / 2. If the egg breaks, then we know that the critical floor _f_ is below _n_ / 2; if the egg does not break, then then _f_ is above _n_ / 2. This essentially reduces the number of floors which we would have to test in half. Then, with the remaining section, we could find the halfway point of that section and test what happens to the egg at that floor, which would again reduce the number of floors to test by half. This loop would essentially be repeated over and over again until the floor is found. The algorithm would have to recursively divide the floors in half each time, so the runtime complexity would be O(log n) with a base of 2.