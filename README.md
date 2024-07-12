# -FIBONACCI-GENERATOR-Python
Fibonacci Sequence Generator  My first Git repository! This simple Python script generates infinite Fibonacci numbers, perfect for beginners learning about generators and the yield statement.


# Introduction:

The Fibonacci sequence is a series of numbers where each number is the sum of the two preceding ones, usually starting with 0 and 1. This script demonstrates how to generate an infinite Fibonacci sequence using Python's generator functionality.

# Features:

Generates an infinite Fibonacci sequence
Uses a simple and efficient generator function
Includes examples of printing the sequence to the console and saving it to a file
Easy to understand and modify for learning purposes
Installation
To use this script, you'll need Python installed on your machine. You can download Python from the official Python website.

Clone this repository to your local machine using:
git clone https://github.com/faqhus/-FIBONACCI-GENERATOR-Python.git

# Usage:

Generating and Printing Fibonacci Numbers
You can run the script to generate and print the first 20,000 Fibonacci numbers:

def infinite_fibonacci():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

fib_gen = infinite_fibonacci()
for _ in range(20000):
    print(next(fib_gen))


"Saving Fibonacci Numbers to a List"
If you want to save the Fibonacci numbers to a list:
def infinite_fibonacci():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

fib_gen = infinite_fibonacci()
fibonacci_numbers = [next(fib_gen) for _ in range(20000)]
print(fibonacci_numbers[:10])

Saving Fibonacci Numbers to a File:

To save the Fibonacci numbers to a file:


def infinite_fibonacci():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

fib_gen = infinite_fibonacci()
with open('fibonacci_numbers.txt', 'w') as file:
    for _ in range(20000):
        file.write(f"{next(fib_gen)}\n")

# Contributing:
I welcome contributions to this project! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

# Contact
If you have any questions or feedback, feel free to reach out to me:

Name: Faqir Hussain
Email: faqhuss@gmail.com
GitHub: faqhus
Thank you for checking out my project!

# Author: Faqir Hussain
