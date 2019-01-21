Lists, Tuples and Sets.

In lists to access the last element without knowing the length of the list. It is better to use the -1 as index.

list_name[-1]

>>> a=[1,2,3]
>>> a.append(4)
>>> a
[1, 2, 3, 4]
>>> a.insert(0,"The list elements are")
>>> a
['The list elements are', 1, 2, 3, 4]
>>> b=[5,6,7,8]
>>> a.extend(b)
>>> a
['The list elements are', 1, 2, 3, 4, 5, 6, 7, 8]
>>> a.remove('The list elements are')
>>> a
[1, 2, 3, 4, 5, 6, 7, 8]
>>> a.insert(0,"The list elements are")
>>> a.remove('The list elements Are')
Traceback (most recent call last):
  File "<pyshell#47>", line 1, in <module>
    a.remove('The list elements Are')
ValueError: list.remove(x): x not in list
>>> a.remove('The list elements are')
>>> a.pop()
8
>>> a
[1, 2, 3, 4, 5, 6, 7]

>>> a.reverse()
>>> a
>>> [7, 6, 5, 4, 3, 2, 1]
>>> a.sort(reverse=True)
>>> a
>>> [7, 6, 5, 4, 3, 2, 1]
>>> a.sort()
>>> a
>>> [1, 2, 3, 4, 5, 6, 7]
>>> a.sort(reverse=True)
>>> a
>>> [7, 6, 5, 4, 3, 2, 1]

sorted will not alter the original list
min,max,sum functions.

>>> a.find(5)
Traceback (most recent call last):
  File "<pyshell#59>", line 1, in <module>
    a.find(5)
AttributeError: 'list' object has no attribute 'find'
>>> a.index(5)
2

find function is used for strings but not the list.

>>> b=['a','c','d']
>>> ''.join(b)
'acd'


Tuples:
Immutable

>>> a=(1,)
>>> a[0]=2
Traceback (most recent call last):
  File "<pyshell#81>", line 1, in <module>
    a[0]=2
TypeError: 'tuple' object does not support item assignment

Sets:

It is optimised to check the membership of the item.
Order of the element in the set varies.

>>> a={1,2,3,4}
>>> b={1,2,5,6}
>>> a.intersection(b)
{1, 2}
>>> a.union(b)
{1, 2, 3, 4, 5, 6}
>>> a.difference(b)
{3, 4}


empty_list=[]
empty_list=list()

empty_tuple=()
empty_tuple=tuple()

empty_set={}#this isnot right , it creates dictionary.
empty_set=set()