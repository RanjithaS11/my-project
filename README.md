# my-project
def fibonacci_iterative(n):
    """
    Generates a Fibonacci sequence up to n terms using iteration.

    Args:
        n: The number of terms in the sequence.

    Returns:
        A list containing the Fibonacci sequence.
    """
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    else:
        list_fib = [0, 1]
        while len(list_fib) < n:
            next_fib = list_fib[-1] + list_fib[-2]
            list_fib.append(next_fib)
        return list_fib

# Example usage:
num_terms = 10
print(fibonacci_iterative(num_terms))
