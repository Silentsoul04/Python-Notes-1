LEGB rule
Local Enclosing Global Built-in

If the variable is called in the main function, it first checks for the local declaration of the variables, if not it checks for the global declaration, and if not it checks for the built in variables.

>>> x= 'x is global'
>>> def tst():
	    x='x is local'
	    print(x)


>>> tst()

x is local
>>> print(x)

x is global
	    
>>> def tst():
	    print(x)


>>> tst()

x is global
>>> def tst():
	    global x
	    x='x is local'
	    print(x)


>>> tst()

x is local
>>> print(x)

x is local


x= 'x is global'

def tst():
    global x
    #x='x is local'
    print(x)

tst()    
print(x)

Output:
x is global

x= 'x is global'

def outertst():
    x='x is outer'
    def innertst():
        nonlocal x
        x='x is inner'
        print(x)
    innertst()
    print(x)
    
outertst()

output:
x is inner
x is inner
