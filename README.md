#Generate the first 100 Fibonacci numbers.
#Use a plotting library to visualize the numbers.

import matplotlib.pyplot as plt

#Function to generate fibonacci numbers
def fibonacci(n):
    fib_seq=[0,1]
    for i in range(2,n):
        fib_seq.append(fib_seq[-1] + fib_seq[-2])
    return fib_seq

fib_numbers=fibonacci(100)

#Plotting the Fibonacci series
plt.figure(figsize=(10,5))
plt.plot(fib_numbers, marker='o')
plt.title('First 100 Fibonacci Numbers')
plt.xlabel('Index')
plt.ylabel('Fibonacci Number')
plt.grid()
plt.show()
