<<<<<<< HEAD


# Decorators(preetha)

- Functions are passed as arguements.
```
def my_decorator(func):
    def wrapper():
        print("Wrapper function is beginning to be executed")
        func()
        print("Function has been executed")
    return wrapper

@my_decorator
def print_hi():
    print("Hi!")
```

-  @my_decorator is just an easier way of saying print_hi = my_decorator(print_hi).

**Decorators :**(aditya)

* A decorator is a function that takes a function as argument, performs some tasks without altering the source code of the passed function and returns another function.
* Use : adding additional functionality to a function without modifying its code.

![decorators1](images/decorators1.PNG) 

* Instead of writing the last two lines, the more commonly used syntax is as follows:

![decorators2](images/decorators2.PNG) 

* When the arguments are present in the original function, the wrapper function and the original function must have the args and kwargs.
(lalith)
1. First class functions:- allow us to treat functions like any other object.

   eg:- we can pass functions as an arguments to other functions, return functions, assign functions to variables etc. 

   Closures:- allow us to take advantage of first-class functions and return an inner function that remembers and has access to variables local to the scope in which they were created.

   eg:-here message variable is free variable.![1547980913051](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547980913051.png) 

   ![1547980931986](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547980931986.png) 

   here it prints message variable several times, that is called as closure. It remembers message variable even after the outer function is finished executing.

   ![1547981168797](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547981168797.png) 

   

2. **Decorators:-** it is a function that takes functions as arguments, perform some **functionality** and returns a function.

   ![1547981412382](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547981412382.png) 

   or

   ![1547981571530](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547981571530.png) 

3. ![1547981800834](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547981800834.png) 

   when passing two functions to single decorator function, use positional and keyword arguments as shown above.

4. **classes as decorators:-**

   ![1547981921202](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547981921202.png) 

5. **Practical examples of decorators:-**

   One of the common use cases for decorators in python is logging. It maintains info regarding how many times a function is called and what are the arguments passed into that function. 

   code:-

   ![1547982530448](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982530448.png) 

   ![1547982566257](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982566257.png) 

   once it is executed a log file is created and it has 

   ![1547982388871](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982388871.png) 

   

6. **Timing how long the function should run** is another use of decorator.

   eg:- 

   ![1547982597068](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982597068.png) 

   ![1547982629013](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982629013.png) 

7. another example:-using decorators for single function

   ![1547982716661](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982716661.png) 

   if the order is switched then it will run as we need it.

   ![1547982757966](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982757966.png) 

   hence it didn't print the info in log file but created a wrapper file and the info is present in that file but not in log file as in above case before switching decorators.

   ![1547982854474](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547982854474.png) 

8. watch video from 24 to 30 for another example.

=======
#Decorators are used to add functionality to the original function.



def decorator(original):
    def wrapp():
        print('Inside the wrapp {}'.format(original.__name__))
        return original()
    return wrapp

def output():
    print("Function executed")

my_dec=decorator(output)

my_dec()

Output:

Inside the wrapp output
Function executed

Can be declared as follows

def decorator(original):
    def wrapp():
        print('Inside the wrapp {}'.format(original.__name__))
        return original()
    return wrapp

@decorator
def output():
    print("Function executed")

output()




def decorator(original):
    def wrapp(*args,**kwargs):
        print('Inside the wrapp {}'.format(original.__name__))
        return original(*args,**kwargs)
    return wrapp

@decorator
def output():
    print("Function executed")
@decorator
def output_info(empno,age):
    print('Function executed with arguments {} {}'.format(empno,age))

output_info(1081916,22)






def decorator(original):
    def wrapp(*args,**kwargs):
        print('Inside the wrapp {}'.format(original.__name__))
        return original(*args,**kwargs)
    return wrapp


class decorator_class(object):
    def __init__(self,original):
        self.original=original
    def __call__(self,*args,**kwargs):
        print('Inside the call method {}'.format(self.original.__name__))
        return self.original(*args,**kwargs)


@decorator_class
def output():
    print("Function executed")
@decorator_class
def output_info(empno,age):
    print('Function executed with arguments {} {}'.format(empno,age))

output_info(1081916,22)
>>>>>>> origin/prvnrj_notes

