# Decorators

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