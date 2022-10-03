# In Tests We Trust — TDD( Test-Driven Development) with Python(1)

 ## Unit tests 

### Baby steps :

 example :
 input >name (lujain)
 output >gender(female)

 
 1. for  test name 
 The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.

2. The test file name should follow the same name of module name. For instance, if our module is gender.py, our test name should be test_gender.py. It’s ideal to separate the tests folder from production code (the implementation) and to have something like this:

```
mymodule/
 — module.py
 — another_folder/
 — — another_module.py
tests/
 — test_module.py
 — another_folder/
 — — test_another_module.py
```

**more thing, focus here**
 A convention widely used is the **AAA**: Arrange, Act and Assert.

* Arrange: you need to organize the data needed to execute that piece of code (input);
* Act: here you will execute the code being tested (exercise the behaviour);
* Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

### The cycle
* 🆘 Write a unit test and make it fail 
* ✅ Write the feature and make the test pass! 
* 🔵 Refactor the code

# What does the if __name__ == “__main__”: do?(2)
1. Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
2. If you import this script as a module in another script, the __name__ is set to the name of the script/module.
3. Python files can act as either reusable modules, or as standalone programs.
4. if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.


# Introduction to Recursion – Data Structure and Algorithm Tutorials(3)

**What is Recursion?** The process in which a function calls itself directly or indirectly

```
int fact(int n)
{
    if (n < = 1) // base case
        return 1;
    else    
        return n*fact(n-1);    
}
```
**How are recursive functions stored in memory?**

Recursion uses more memory, because the recursive function adds to the stack with each recursive call, and keeps the values there until the call is finished. The recursive function uses LIFO (LAST IN FIRST OUT) Structure just like the stack data structure.
**How memory is allocated to different function calls in recursion?**
When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to the calling function and a different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.

# Thing I need to know abour more
* TDD

# Refrences
1. Gomes, A. P. (2018, June 20). In Tests We Trust — TDD with Python - Code Like A Girl. Medium. Retrieved October 3, 2022, from [link](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

2. GeeksforGeeks. (2020, December 11). What does the if __name__ == “__main__”: do? Retrieved October 3, 2022, from [link](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

3. GeeksforGeeks. (2022, September 19). Introduction to Recursion - Data Structure and Algorithm Tutorials. Retrieved October 3, 2022, from[link](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)