Exercise I

a) The running time is O(n). The number of times the while loop runs depends on the value of n, and there are no other loops inside of the while loop. 

b) The running time is O(n^3). For every loop except the last, the number of time the function executes depends on n, and n must be multiplied by n for each nested loop. However, since the number of times the final loop depends on a constant, that term can ultimately be dropped as insignificant.