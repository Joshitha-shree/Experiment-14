# Experiment-14
### Name: JOSHITHA SHREE BS
### Register Number: 212224230107

## Pytest Python program for Fibonacci Series 
# Aim:To write a python program for Fibonacci Series and test the test cases using Pytest. 
# Algorithm: 
Step 1: Write the python program for Fibonacci Series.
Step 2: Make sure that function name should be “def test_*():” and the line to be tested
should have assert keyword at the beginning.
Step 3: Write some test cases for to be tested and save it as “test_fib.py”.
Step 4: Open command prompt and change the directory to where pytest and program is
saved and type “pytest test_fib.py” and run it.
Step 5: Stop the program. 
# Program
fibonacci.py
```
def fibonacci(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    elif n == 2:
        return [0, 1]

    series = [0, 1]
    for i in range(2, n):
        series.append(series[-1] + series[-2])
    return series

```
test_fib.py
```
# test_fib.py
from fibonacci import fibonacci

def test_fibonacci_zero():
    assert fibonacci(0) == []

def test_fibonacci_one():
    assert fibonacci(1) == [0]

def test_fibonacci_two():
    assert fibonacci(2) == [0, 1]

def test_fibonacci_five():
    assert fibonacci(5) == [0, 1, 1, 2, 3]

def test_fibonacci_ten():
    assert fibonacci(10) == [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```
# Output
<img width="1285" height="254" alt="image" src="https://github.com/user-attachments/assets/d0e6d967-5352-4514-901a-24fb599471ca" />

# Result
Thus,the Fibonacci series program was successfully implemented in Python and verified using Pytest test cases.
