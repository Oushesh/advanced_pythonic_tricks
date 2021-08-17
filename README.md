## advanced_pythonic_tricks
Descriptions of Recursive DFS, Stackoverflow, increasing stack limit, rewriting in Iterative Approach, Y Combinators and ZCombinators

* https://stackoverflow.com/questions/50974371/efficient-dynamic-programming-using-python
* https://stackoverflow.com/questions/49210801/python3-pass-lists-to-function-with-functools-lru-cache
* The clean way: modifying the Y Combinator
* https://stackoverflow.com/questions/13591970/does-python-optimize-tail-recursion?rq=1
* https://stackoverflow.com/questions/34115298/how-do-i-get-the-current-depth-of-the-python-interpreter-stack
* https://stackoverflow.com/questions/49091751/delaying-evaluation-with-abstractions-in-the-y-combinator


Example einsum.
s = 0
n, m = A.shape
for i in range(n):
    for j in range(m):
        s += A[i, j]*B[i, j]
        
# Using built-in numpy functions
np.trace(np.dot(A.T, B))

# Using einsum
np.einsum('ij,ij->', A,B)
