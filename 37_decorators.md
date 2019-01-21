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

