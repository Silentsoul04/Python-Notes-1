
Enumerate function:

>>> list1=["b","p","r"]
>>> 
>>> for i in enumerate(list1):
	print(i)

	
(0, 'b')
(1, 'p')
(2, 'r')
>>> for i,value in enumerate(list1):
	print(i,value)

	
0 b
1 p
2 r
>>> for i,value in enumerate(list1,100):
	print(i,value)

	
100 b
101 p
102 r


file_name.py

import file_name

variable=file_name.function_name()
variable=file_name.variable_name()

import file_name as fn

variable=fn.function_name()
variable=fn.variable_name()

from file_name import function_name,variable_name

variable=function_name()
variable=variable_name()

import random,math,datetime

random.choice()

if the files are in another directories then we are supposed to add the paths using sys.path.append()

instead we Can change the environment variable!! computer->system->advanced system settings->environment variable-> Give PYTHONPATH, And the path of the folder that resides.

