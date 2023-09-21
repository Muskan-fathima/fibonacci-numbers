def fibonacci_iterative(n):
    fib = [0, 1]
    for i in range(2, n):
        next_fib = fib[i - 1] + fib[i - 2]
        fib.append(next_fib)
    return fib[:n]
n = int(input("Enter the number of Fibonacci numbers to generate: "))
fibonacci_sequence = fibonacci_iterative(n)
print(f"Fibonacci sequence of {n} numbers: {fibonacci_sequence}")
