li.sort()
li.sort(reverse=True)
sorted_list=sorted(li)
rev_list=sorted(li,reverse=True)

In tuples and dictionaries we don't have sort(), only sorted() works..!!
In dictionaries sorting is for the keys.

d={2:'b',1:'a',3:'c'}
>>> d.sort()
Traceback (most recent call last):
  File "<pyshell#1>", line 1, in <module>
    d.sort()
AttributeError: 'dict' object has no attribute 'sort'
>>> sorted(d)
[1, 2, 3]
li=[-6,-5,-4,1,2,3]
>>> li.sort(key=abs)

>>> li
[1, 2, 3, -4, -5, -6]

OBJECTS:

class Employee():
	def __init__(self,name,age,salary):
		self.name=name
		self.age=age
		self.salary=salary
	def __repr__(self):
		return '({},{},${})'.format(self.name,self.age,self.salary)
		
e1=Employee('praveen',20,40000)
e2=Employee('Raja',21,42000)
e3=Employee('BprvnRj',22,80000)
employees=[e1,e2,e3]
def e_sort(emp):
	return emp.name
e=sorted(employees,key=e_sort)
or
e=sorted(employees,key=lambda e:e.name)
or 

from operator import attrgetter
e=sorted(employees,key=attrgetter('name'))



e=[e1,e2,e3]

