DECORATOR WITH ARGUMENTS

def prefix_decorator(prefix):
    def decorator(original):
        def wrapp(*args,**kwargs):
            print(prefix,'Before {}'.format(original.__name__))
            result= original(*args,**kwargs)
            print(prefix,'After {}'.format(original.__name__))
            return result
        return wrapp
    return decorator


'''class decorator_class(object):
    def __init__(self,original):
        self.original=original
    def __call__(self,*args,**kwargs):
        print('Inside the call method {}'.format(self.original.__name__))
        return self.original(*args,**kwargs)'''

'''@decorator_class
def output():
    print("Function executed")'''
@prefix_decorator('TESTING:')
def output_info(empno,age):
    print('Function executed with arguments {} {}'.format(empno,age))

output_info(1081916,22)

