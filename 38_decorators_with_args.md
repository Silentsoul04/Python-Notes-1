# Decorators with arguements

```
def do_twice(func):
    def wrapper_do_twice(*args, **kwargs):
        func(*args, **kwargs)
        func(*args, **kwargs)
    return wrapper_do_twice
```

- The wrapper_do_twice() inner function now accepts any number of arguments and passes them on to the function it decorates.