

# Decorators with arguements(preetha)

```
def do_twice(func):
    def wrapper_do_twice(*args, **kwargs):
        func(*args, **kwargs)
        func(*args, **kwargs)
    return wrapper_do_twice
```

- The wrapper_do_twice() inner function now accepts any number of arguments and passes them on to the function it decorates.

**Decorators with arguments :**(aditya)

* Whenever there's a need to pass arguments, to the decorator function, nest it into one more level and pass the arguments to that outer function, which could be used by the previous decorator function and the further nested ones.

![decorators_args](images/decorators_args.PNG)  

(lalith)
![1547983321767](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547983321767.png) 

![1547983450703](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547983450703.png)

