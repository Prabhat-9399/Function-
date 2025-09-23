Functions Assignment
1. What is the difference between a function and a method in Python?
Function and method, both are resuable code that performs specefic task, but differ in how they are called.

Function - is defined using the def keyword. It can exist independently of any class or any object

Method - method is also defined, using the def keyword, but inside the class. It automatically takes the instance (self) or (class) as the first argument.

2. Explain the concept of function arguments and parameters in Python
Parameters - are the variables defined inside the function's parantheses. They act as placeholders for the values, the function wil receive when its called. Example - def greet(name): # 'name' is a parameter print("Hello,", name)

Arguments - are the actual values you passs to the function when calling it. Example - greet("Priya") # "Priya" is an argument

3. What are the different ways to define and call a function in Python?
Function in python can be defined and called in several ways like-

Simple Function with no parameters def greet(): print("Hello, World!")

Function with parameters def greet(name): print("Hello,", name)

Function with default parameters def greet(name="Guest"): print("Hello,", name)

4. What is the purpose of the return statement in a Python function?
The return function is used to send a result back to the caller. Without return a function will always return, none be default Example - def add(a, b): return a + b

result = add(5, 3) print(result) # 8

5.What are iterators in Python and how do they differ from iterables?
Iterable - is any python object, that can return its elements one at a time. Like- lists, tuples, strings, dictionaries and sets. An iterable is an object that impliments the iter method.

Iterator- An Iterator is an object that actually produces the next value when you ask for it. iter() - returns the iterator object itself. next() - returns the next element It produces the elements one by one.

6. Explain the concept of generators in Python and how they are defined.
A generator in python is a type of iterator, that allows you to produce one value at a time using the yield keyword, instead of creating and storing the whole collection in memory.

Example - def countdown(n): while n > 0: yield n n -= 1

7.What are the advantages of using generators over regular functions?
Regular functions that return a list, build the entire list in memory before returning it. Generators produce items one at a time, only when needed. Also since generators dont compute everything at once, they start producing results immidiately.

8. What is a lambda function in Python and when is it typically used?
A lambda function in python is a small, anonymous function defined using the lambda keyword. It can only contain one expression.

9. Explain the purpose and usage of the map() function in Python.
The map() function is used to apply a function to each item in an iterable list and return a new map object. Example- nums = [1, 2, 3, 4]

def square(x): return x**2

result = map(square, nums) print(list(result)) # [1, 4, 9, 16]

10. What is the difference between map(), reduce(), and filter() functions in Python?
map()- apply a function to each item in iterable and return a new iterable.

filter()- filter elements in an iterable based on condition (True/False)

reduce()- reduce an iterable to a single cumulative value by repeatedly applying a function.
11.
![Image](https://github.com/user-attachments/assets/1285551b-b657-4956-ac0e-a54542b62382)
practical questions 
1.Write a Python function that takes a list of numbers as input and returns the sum of all even numbers in the list.
