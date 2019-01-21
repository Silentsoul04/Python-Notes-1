Functions
'pass' keyword will help to skip the functions 
It will not throw any errors if we call the function.

args and kwargs keywords!!
args takes the arguments whereas kwargs the key-value pairs..

def hello(*args,**kwargs):
	print(args)
	print(kwargs)

>>> hello('hi')
('hi',)
{}
>>> hello(1,2,3,4)
(1, 2, 3, 4)
{}
>>> hello(1,key="value")
(1,)
{'key': 'value'}
>>> hello(1,key="value",2)
SyntaxError: positional argument follows keyword argument
>>> hello(1,2,key="value")
(1, 2)
{'key': 'value'}