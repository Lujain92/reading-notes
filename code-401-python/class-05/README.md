# OOP
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic.

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

**Why classes?**

You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class. For instance, if we were to define another object with the "MyClass" class and then change the string in the variable above:
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
myobjecty = MyClass()

myobjecty.variable = "yackity"

# Then print out both values
print(myobjectx.variable)
print(myobjecty.variable)

>> output:
blah
yackity
```
# Thinking Recursively in Python
Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve. This is the essence of thinking recursively.

A recursive function is a function defined in terms of itself via self-referential expressions.

This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

Notes About Recursion

* Python doesn’t have support for tail-call elimination. As a result, you can cause a stack overflow if you end up using more stack frames than the default call stack depth => 3000.

* Python’s mutable data structures don’t support structural sharing, so treating them like immutable data structures is going to negatively affect your space and GC (garbage collection) efficiency because you are going to end up unnecessarily copying a lot of mutable objects.


# Python Testing with pytest: Fixtures and Coverage

**Fixtures**

When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".

But in other cases, things are a bit more complex. You'll want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world, and they take a variety of different forms.

In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.

## things I need to lnow about more
* OPP

## Refrences

1. Classes and Objects, learnpython.org, accessed 10 October 2022, https://www.learnpython.org/en/Classes_and_Objects

2. Abhirag Awasthi, May 27, 2018, Thinking Recursively in Python, realpython.com, accessed 10 October 2022, https://realpython.com/python-thinking-recursively/

3. Reuven M. Lerner, Jan 14, 2019, Python Testing with pytest: Fixtures and Coverage, linuxjournal.com, accessed 10 October 2022, https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage