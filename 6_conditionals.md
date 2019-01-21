`Python` evaluates true or false using if, else and elif statements.
if condition:
	...
elif condition:
	...
else:
	...

Comparision operators

==
!=
>
<
>=
<=

and
not 
or
is

The operators "==" are different from "is".

code and output:

>>> a=[1,2,3]
>>> c=[1,2,3]
>>> print(a==c)
True
>>> print(a is c)
False

Because "is" operator compares the memory id of a and c.

>>> print(id(a))
63816248
>>> print(id(c))
59433448
>>> b=c
>>> print(id(b),id(c),b==c)
59433448 59433448 True

False values:
The kind of sequences which leads to the false values are as follows

False, None, zero, [],(),{},''

>>> string=''
>>> if string:
	print("It's there")
else:
	print("Nothing is present :/")

	
Nothing is present :/

