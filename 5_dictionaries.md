Dictionaries

Instead of using indexing method to access the key-value pairs, it is better to use the get method to access the key-value. If incase key-value is not available, this get method function returns the None.

>>> d={1:'a',2:'b'}
>>> d.get(1)
'a'
>>> d.get(3)
>>> d[3]='c'
>>> d
{1: 'a', 2: 'b', 3: 'c'}
>>> d.update(1:'A',2:'B',3:'C')
SyntaxError: invalid syntax
>>> d.update(1='A',2='B',3='C')
SyntaxError: keyword can't be an expression
>>> d.update({1:'A',2:'B',3:'C'})
>>> d
{1: 'A', 2: 'B', 3: 'C'}
>>> d.get(4,"Not found")
'Not found'
>>> del d[2]
>>> d
{1: 'A', 3: 'C'}
>>> d.update({1:'A',2:'B',3:'C'})
>>> popped=d.pop()
Traceback (most recent call last):
  File "<pyshell#104>", line 1, in <module>
    popped=d.pop()
TypeError: pop expected at least 1 arguments, got 0
>>> popped=d.pop(2)
>>> d
{1: 'A', 3: 'C'}
>>> d.update({1:'A',2:'B',3:'C'})
>>> d.keys()
dict_keys([1, 3, 2])
>>> d.values()
dict_values(['A', 'C', 'B'])
>>> d.items()
dict_items([(1, 'A'), (3, 'C'), (2, 'B')])
>>> for key in d:
	print(key)

	
1
3
2
>>> for key,values in d.items():
	print(key,value)

	
Traceback (most recent call last):
  File "<pyshell#116>", line 2, in <module>
    print(key,value)
NameError: name 'value' is not defined
>>> for key,values in d.items():
	print(key,values)

	
1 A
3 C
2 B
>>> for key in d:
	print(d[key])

	
A
C
B
>>>