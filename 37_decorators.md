**Decorators :**

* A decorator is a function that takes a function as argument, performs some tasks without altering the source code of the passed function and returns another function.
* Use : adding additional functionality to a function without modifying its code.

![decorators1](images/decorators1.PNG) 

* Instead of writing the last two lines, the more commonly used syntax is as follows:

![decorators2](images/decorators2.PNG) 

* When the arguments are present in the original function, the wrapper function and the original function must have the args and kwargs.